# Contributing to This Project

## Contribution Guidelines

1. **Folder Structure and Naming Conventions**:

- Follow the existing folder structure stated in the README and **use semantic and descirptive names** for any files or folders.
- Ensure assets and files are placed in their appropriate directories.
  - `assets/`for media files.
  - `scripts/`for Python scripts or extensions.
  - `comps/` for reusable container components

2. \*\*

- Inside Touchdesigner, rename default nodes to meaningful names reflecting their purpose.

## Node and Network Documentation

- Use comments on important nodes:
  - add shot, descriptive comments using Right-click → add Comment.
  - Include comments within each Base COMP to describe its purpose, inputs, outputs, and internal processes.
  - For reusable components; document their purpose and how to use in comments.

## Testing Requirements

- Before submitting changes, thoroughly test your modifications:
  - Verify the project runs smoothly at a stable frame rate.
  - Test new nodes, components, or features to ensure they are functioning as intended and compatible with existing systems.

## Dependencies

- Avoid adding unnecessary dependencies. If new dependencies (e.g., Python libraries or assets) are required, ensure:
  - They are documented in the project’s setup instructions or a dedicated DEPENDENCIES.md file.
  - They are included in the repository (if possible) or instructions for installing them are provided.

## Branching Strategy

1. **_Main Branch_**

   - The main branch contains stable, production-ready project files.

2. **_Develop Brnach_**

   - The branch where features are added to and tested before mergin to the Main branch.

3. **_Feature Branches_**
   - Create a new branch for each feature:
   - Name feature branches as feature/[name].
   - Once the feature or fix is complete, submit a pull request to merge it into the main branch.

## Commit Guidelines

- Use clear and descriptive commit messages.
- Use the following commit prefixes:
  - `feat: [description]` for new features.
  - `fix: [description]` for bug fixes.
  - `chore: [description]` for maintenance tasks.
  - `refractor: [description]` for clean up or improvements.
  - `docs: [description]` for markdown files.

## Pull Requests

1. **Coding Conventions**

   - Adhere to the project conventions outlined in CONVENTIONS.md (if applicable).
   - Maintain readability and modular design principles when adding or editing nodes and networks.
   - Ensure reusable components (Base COMPs) are encapsulated with clear inputs/outputs and optional parameters.

2. **Pull Request Description**

When creating a pull request, include the following: - Summary of Changes: Explain what you’ve done and why. - Testing Steps: Describe how to test the new functionality or verify the bug fix.

3. **Review Process**
   -All pull requests will be reviewed for: - Consistency with project conventions. - Proper testing and stable performance. - Clear documentation of new features or fixes.

## Additional Notes

1. **Modular Design:**

   - Ensure new features or fixes are encapsulated in reusable and modular Base COMPs when possible.
   - Use custom parameters and exposed inputs/outputs for flexible usage.

2. **Asset Management:**

   - Organize assets (e.g., textures, videos, audio) into appropriate subfolders under assets/.
   - Use relative paths for file references to maintain project portability.

3. **Task Management:**

   - Track and update task progress on the project’s task board.
   - Move completed tasks to “Done” after submitting a pull request or merging changes.

4. **Community Contributions:**
   - Contributions of all levels are welcome, from small bug fixes to major feature implementations.
   - If you are unsure about a change, open a discussion or issue in the repository to gather feedback.

## Thank You for Contributing!

By adhering to these guidelines, you help ensure the project remains high-quality, easy to maintain, and accessible for other contributors. Let us know if you have any questions-happy **creating!**
