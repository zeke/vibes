# Surfing with Claude: Automated Web Browsing with Claude Code and Playwright MCP

This tutorial shows you how to use Claude Code with the Playwright MCP server to perform fully automated and intelligent web surfing directly from your terminal.

## Demo Video

Watch a live demonstration of Claude Code with Playwright MCP in action: [https://youtu.be/0AX3z5dA4EY](https://youtu.be/0AX3z5dA4EY)

## Installation

First, install Node.js from [https://nodejs.org](https://nodejs.org) and verify it's working:

```bash
node --version
npm --version
```

Install Claude Code, Anthropic's official CLI:

```bash
npm install -g @anthropic-ai/claude-code
claude --version
```

Add the Playwright MCP server to Claude Code:

```bash
claude mcp add playwright npx '@playwright/mcp@latest'
```

## Configuration

### Verify MCP Server Connection

Start Claude Code and check that the Playwright server is available:

```bash
claude
```

Then ask Claude:
```
What MCP tools do you have available?
```

You should see Playwright-related tools in the response.

## Using Playwright MCP for Web Surfing

### Basic Commands

Once configured, you can ask Claude to perform various web browsing tasks:

#### 1. Navigate to a Website
```
Navigate to https://example.com and tell me what you see
```

#### 2. Take Screenshots
```
Go to https://github.com and take a screenshot
```

#### 3. Fill Out Forms
```
Go to the GitHub login page and show me the form fields
```

#### 4. Extract Information
```
Visit https://news.ycombinator.com and list the top 5 stories
```

#### 5. Click Elements and Navigate
```
Go to Wikipedia, search for "artificial intelligence", and summarize the first paragraph
```

### Advanced Examples

#### Web Scraping
```
Visit https://example-shop.com and extract all product names and prices
```

#### Multi-Step Navigation
```
1. Go to Google
2. Search for "Claude AI"
3. Click the first result
4. Take a screenshot
5. Extract the main heading
```

#### Form Automation
```
Navigate to the contact form at https://example.com/contact and fill it with:
- Name: John Doe
- Email: john@example.com
- Message: This is a test message
Then show me a screenshot before submitting
```

#### Testing Web Applications
```
Visit my localhost:3000 app, click the "Login" button, and verify the login form appears
```

## Tips and Best Practices

### 1. Be Specific
Provide clear instructions about what elements to interact with:
```
Click the blue "Submit" button in the top right corner
```

### 2. Use Verification Steps
Ask Claude to confirm actions:
```
Navigate to the checkout page and tell me what fields are required before filling them
```

### 3. Handle Dynamic Content
For sites with dynamic content, specify wait conditions:
```
Go to the dashboard and wait for the charts to load, then describe what data is shown
```

### 4. Save Screenshots
Keep evidence of automated actions:
```
After completing the form, take a screenshot and save it as form-completed.png
```

### 5. Error Handling
Claude will report if elements can't be found or actions fail:
```
Try to click the "Subscribe" button, and if it doesn't exist, look for "Sign Up" instead
```

## Common Use Cases

### Research Automation
```
Visit 5 different news sites and compile a summary of today's top technology headlines
```

### Price Comparison
```
Check the price of [product name] on Amazon, Best Buy, and Walmart, then create a comparison
```

### Content Monitoring
```
Go to my competitor's blog at [URL] and list their 3 most recent posts with publish dates
```

### Form Testing
```
Test the registration form at [URL] with various inputs and identify any validation issues
```

### Documentation Generation
```
Navigate through all pages in the settings menu of [web app] and document each available option
```

## Troubleshooting

### MCP Server Not Found
If Claude can't access Playwright tools:
1. Verify npm installation: `npm --version`
2. Reinstall the server: `npm install -g @modelcontextprotocol/server-playwright`
3. Restart Claude Code

### Browser Launch Failures
If the browser won't start:
1. Check system resources (RAM/CPU)
2. Try headless mode by asking: "Navigate to [URL] in headless mode"
3. Update Playwright: `npm update -g @modelcontextprotocol/server-playwright`

### Element Not Found Errors
If Claude can't find elements:
1. Ask for a screenshot first to see the current page state
2. Use more specific selectors: "Click the button with text 'Submit' inside the form"
3. Add wait instructions: "Wait for the page to fully load, then click..."

## Security Considerations

- Never use this for accessing sensitive accounts without proper authorization
- Avoid automating actions on sites that prohibit automated access
- Don't store credentials in prompts; use environment variables when needed
- Be aware that screenshots may capture sensitive information

## Conclusion

Claude Code with Playwright MCP transforms your terminal into a powerful web automation tool. You can surf the web, extract data, fill forms, and test web applications all through natural language commands. The combination of Claude's intelligence and Playwright's browser automation creates endless possibilities for web interaction automation.

Start simple with basic navigation and screenshots, then gradually explore more complex multi-step workflows as you become comfortable with the system.