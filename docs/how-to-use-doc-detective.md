

  # How to Use Doc Detective

Doc Detective is a versatile tool for automating documentation testing and coverage analysis. Here's a guide on how to use it:

1. **Installation**: 
   - Install Doc Detective via npm: `npm install -g doc-detective`

2. **Configuration**:
   - Create a `.doc-detective.json` file in your project root to configure settings.
   - Set up environment variables in a `variables.env` file if needed.

3. **Writing Tests**:
   - Create test specifications in JSON format (e.g., `test.spec.json`).
   - Define tests with steps using actions like `goTo`, `find`, `typeKeys`, etc.
   - You can also embed tests in Markdown files using special comment syntax.

4. **Running Tests**:
   - Execute tests using the command: `doc-detective runTests`
   - Specify input files or directories using the `--input` flag.
   - Use `--output` to define where results should be saved.

5. **Coverage Analysis**:
   - Run coverage analysis with: `doc-detective runCoverage`
   - This helps identify untested parts of your documentation.

6. **Inline Tests in Markdown**:
   - Use `[comment]: # (test start {...})` to begin a test block.
   - Define steps with `[comment]: # (step {...})`.
   - End the test with `[comment]: # (test end)`.

7. **Automated Actions**:
   - Use actions like `checkLink`, `httpRequest`, `saveScreenshot` to automate various testing tasks.

8. **Context Settings**:
   - Define different contexts (browsers, platforms) in your config file for comprehensive testing.

9. **Customization**:
   - Adjust settings like `logLevel`, `recursive`, and `detectSteps` in your config file.

10. **Integration**:
    - Integrate Doc Detective into your CI/CD pipeline for continuous documentation testing.

Remember to refer to the [Doc Detective documentation](https://doc-detective.com) for detailed information on schemas, actions, and advanced usage.

  