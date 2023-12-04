# Fork of BrowserGPT by Produvia

This is a fork of the BrowserGPT project, originally developed by mayt. The primary focus of this version is to enhance its performance and usability specifically for LinkedIn. This adaptation optimizes the integration between OpenAI's GPT-4 and the Playwright library to provide a more streamlined experience when navigating and interacting with LinkedIn.

## Key Changes in This Fork

1. **Simplified Text Node Handling**: The text node creation process is simplified, removing checks for JSON text nodes and directly returning the text node.
2. **Removed Default Timeout Setting**: The default 60-second timeout setting for Playwright pages has been removed, which may affect script execution time.
3. **Removed Debugging and Token Length Calculations**: The fork eliminates functions and logs related to calculating and debugging token lengths in the HTML, leading to cleaner code.
4. **Dependency Version Adjustment**: The `@playwright/test` package version is downgraded for improved compatibility and performance.
5. **Streamlined Error Handling and Logging**: The fork simplifies error logging in the GPT query process and removes conditional checks for error objects.

## Areas for Future Improvement

1. **Content Summarization with LLMs**: Integrating models like OpenAI's GPT-4 Turbo could enable the tool to summarize content from web pages more effectively. For instance, it could generate concise summaries of LinkedIn profiles, providing quick insights. This would add significant value to users who need quick information from detailed pages. More about GPT-4 Turbo can be found [here](https://platform.openai.com/docs/models/gpt-4-and-gpt-4-turbo).

2. **Enhanced Navigation with Multi-modal LLMs**: The use of multi-modal LLMs, such as OpenAI's GPT-4V, could revolutionize how the tool interacts with web pages. These models could analyze visual elements to better navigate complex pages. An application could be taking screenshots of specific sections of a LinkedIn profile or identifying and interacting with visual elements more effectively. Learn more about GPT-4V [here](https://platform.openai.com/docs/guides/vision).

3. **Specialized Code Model Workflows for Advanced DOM Interaction**: Developing workflows using models optimized for code generation, like the OpenAI GPT-4 Turbo model, could significantly improve the tool's ability to navigate hidden elements of the DOM. This would be particularly useful for interacting with elements on LinkedIn that are challenging to access with standard prompts or scripts. This approach could lead to more nuanced and effective automation tasks.

## Installation and Usage

The installation and basic usage remain the same as the original BrowserGPT project. Here's a quick overview:

### Install the required packages:

```sh
npm install
```

### Setup

Create a `.env` file in the project root directory and add your OpenAI API key:

```
OPENAI_API_KEY=your_openai_api_key
```

### Running the Script

```sh
npm run start
```

You'll be prompted in the terminal to input tasks using natural language. This fork specifically improves interactions with LinkedIn, so feel free to test LinkedIn-specific commands.

## Limitations

While this fork is optimized for LinkedIn, it inherits the limitations of the original BrowserGPT project. The accuracy and success of tasks may vary depending on the complexity of the web pages and the specificity of the instructions.

## License

This project, like the original BrowserGPT, is licensed under the MIT License. See the LICENSE file for details.
