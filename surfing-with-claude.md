# Surfing with Claude: Automated Web Browsing with Claude Code and Playwright MCP

This tutorial shows you how to use Claude Code with the Playwright MCP server to perform fully automated and intelligent web surfing directly from your terminal.

## What?

- Claude Code is Anthropic's official CLI for Claude. It's a powerful tool that allows you to use Claude's AI capabilities directly from your terminal.
- Playwright is a browser automation tool that allows you to control a browser programmatically.
- Playwright MCP is a server that allows you to use Playwright from Claude Code.


## Demo

Watch a live demonstration of Claude Code with Playwright MCP in action: [https://youtu.be/0AX3z5dA4EY](https://youtu.be/0AX3z5dA4EY)

<a href="https://youtu.be/0AX3z5dA4EY">
  <img src="images/surfing-with-claude.png" alt="Surfing with Claude: Automated Web Browsing with Claude Code and Playwright MCP" width="100%">
</a>

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

## Usage

Time to fire up Claude Code and start surfing!

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