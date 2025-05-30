# 🧪 AI Unit Test Builder for Cursor 🤖

Welcome to **AI Unit Test Builder**! This collection of `.mdc` (Markdown Command) files is designed to systematically generate comprehensive unit tests from your source code using Cursor's AI Agent. Transform your existing functions into well-tested, reliable code through a structured, step-by-step approach.

Stop writing tests manually and let AI analyze your code to generate thorough test suites!

## ✨ The Core Idea

Writing comprehensive unit tests can be time-consuming and often overlooked. This workflow aims to:

1. **Function Analysis:** Automatically identify and analyze all testable functions in your source files.
2. **Systematic Test Generation:** Create focused unit tests for each function, covering various scenarios.
3. **Test Refinement:** Review and improve generated tests through iterative feedback.

This structured approach ensures comprehensive test coverage while maintaining code quality and reliability.

## Workflow: From Source Code to Complete Test Suite 🔍➡️🧪

Here's the step-by-step process using the `.mdc` files in this repository:

### 1️⃣ Extract Functions from Source Code

First, analyze your source file to identify all testable functions and their characteristics.

1. Ensure you have the `extract-functions.mdc` file accessible.
2. In Cursor's Agent chat, initiate function extraction:

   ```
   Use @extract-functions.mdc to analyze @MyComponent.tsx
   ```

   The AI will analyze your source file and create a structured list of all functions with their:
   - Parameters and types
   - Return types
   - Dependencies
   - Complexity indicators
   - Test scenarios suggestions

### 2️⃣ Generate Unit Tests for Each Function

With your function analysis complete, generate comprehensive unit tests for each identified function.

1. Ensure you have `generate-unit-test.mdc` accessible.
2. In Cursor's Agent chat, use the function analysis to create tests:

   ```
   Now use @generate-unit-test.mdc with the function analysis to create tests for MyComponent
   ```

   The AI will generate:
   - Test setup and teardown code
   - Happy path tests
   - Edge case scenarios
   - Error handling tests
   - Mock configurations when needed

### 3️⃣ Review and Refactor Tests

Finally, review the generated tests and refine them for better coverage and maintainability.

1. Create or ensure you have the `refactor-test.mdc` file accessible.
2. In Cursor's Agent chat, refine your tests:

   ```
   Use @refactor-test.mdc to improve the generated tests
   ```

   The AI will:
   - Optimize test structure
   - Remove redundancy
   - Improve test descriptions
   - Add missing test cases
   - Enhance mock implementations

## 🗂️ Files in this Repository

* **`extract-functions.mdc`**: Analyzes source code files to identify all testable functions and their characteristics, creating a structured analysis document.
* **`generate-unit-test.mdc`**: Takes the function analysis and generates comprehensive unit tests for each function, including setup, various test scenarios, and proper assertions.
* **`refactor-test.mdc`**: Reviews and improves generated tests by optimizing structure, adding missing cases, and enhancing overall test quality.

## 🌟 Benefits

* **Comprehensive Coverage:** Ensures all functions are tested with multiple scenarios.
* **Systematic Approach:** Follows a structured process from analysis to implementation.
* **Time Efficient:** Dramatically reduces the time needed to write comprehensive test suites.
* **Quality Assurance:** Generates tests that follow best practices and cover edge cases.
* **Maintainable Tests:** Creates well-structured, readable test code that's easy to maintain.
* **Framework Agnostic:** Works with various testing frameworks (Jest, Vitest, etc.).

## 🛠️ How to Use

1. **Setup:** Place these `.mdc` files in your project's `/mdc/` directory where Cursor can access them.
2. **Follow the Workflow:** Use the three `.mdc` files sequentially as described in the 3-step workflow above.
3. **Customize:** Modify the prompts within the `.mdc` files to match your:
   - Testing framework preferences (Jest, Vitest, etc.)
   - Code style and conventions
   - Specific testing requirements

## 💡 Tips for Success

* **Clean Source Code:** Ensure your source files are well-structured with clear function definitions for better analysis.
* **Specify Testing Framework:** Mention your preferred testing framework (Jest, Vitest, etc.) when starting the process.
* **Review Generated Tests:** Always review and run the generated tests to ensure they work correctly.
* **Iterative Improvement:** Use the refactor step to continuously improve test quality.
* **File Organization:** Keep test files organized alongside their source files (e.g., `Component.tsx` and `Component.test.tsx`).

## 🔧 Supported Features

* **Function Types:** Regular functions, arrow functions, class methods, async functions
* **Testing Frameworks:** Jest, Vitest, Testing Library, and others
* **Mock Generation:** Automatic mock creation for dependencies
* **Edge Cases:** Comprehensive edge case and error scenario testing
* **TypeScript Support:** Full TypeScript analysis and test generation

## 📁 Expected File Structure

```
your-project/
├── mdc/
│   ├── extract-functions.mdc
│   ├── generate-unit-test.mdc
│   └── refactor-test.mdc
├── src/
│   ├── components/
│   │   ├── MyComponent.tsx
│   │   └── MyComponent.test.tsx  # Generated
│   └── utils/
│       ├── helpers.ts
│       └── helpers.test.ts       # Generated
└── tests/
    └── analysis/
        └── function-analysis-MyComponent.md  # Generated
```

## 🤝 Contributing

Have ideas to improve these `.mdc` files or support for additional testing frameworks? Contributions are welcome!

Please feel free to:
* Open an issue to discuss improvements or new features
* Submit a pull request with enhancements
* Share your customized `.mdc` files for different frameworks

## 📋 Example Output

The workflow generates:
1. **Function Analysis Document:** Detailed breakdown of all functions in your source file
2. **Comprehensive Test Files:** Complete test suites with multiple scenarios per function
3. **Refined Test Code:** Optimized, maintainable test implementations

## 🚀 Getting Started

1. Copy the `.mdc` files to your project
2. Choose a source file you want to test
3. Run through the 3-step workflow
4. Review and run your generated tests
5. Iterate and improve as needed

---

Happy test-driven development with AI assistance!
