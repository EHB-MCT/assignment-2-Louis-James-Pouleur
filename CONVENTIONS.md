# Touchdesigner Conventions

## Node Naming Conventions

1. **Meaningful Names**:

- Name nodes desciptively to make the network easy to understand.
  - Example: Use vdeio_input instead of moviefilein1.

2. **Avoid Spaces in Names**:

- Use underscores(\_) or camelCase for names instead of spaces.
  - Example: VideoInput or audio_filter.

3. **Avoid Default Names**:

- Rename nodes from their default names to something relevant
  - Example: null to Count.

## Color Coding Nodes

TouchDesigner allows you to color-code nodes to visually categorize their purpose or function.

- Use consistent color schemes for similar types of nodes, example:
  - Hand tracking: Red
  - Database Posting: Pink
  - Visualising: Blue
- Right-click a node → Node Color → choose a color.

## Network Layout and Organization

1. **Left-To-Right Flow**

- Design networks to flow logically from left to right. place inputs on the left, processing nodes in the middle, and outputs on the right.

2. **Align Nodes**

- Use the grid to align nodes neatly, which makes the network easier to read.

3. **Use Conainers(Base)**

- Use Base COMPs or other container nodes to encapsulate parts of your project. This is especially usefull for modular design and reusable components.

4. **Label Outputs**

- Use the out1 node to label the output of each container so you can easily see where the data exits.

## Python Scripting Conventions

1. **Use op() to Reference Nodes**

- Always use op() for node referencing rather than hardcoding paths.

2. **Comments in Scripts**

- Always comment your scripts to descibe what each section does. This is especially helpful for complex scripts.

## Text in Sections

1. **Add Text to Different Sections**

- Write text in sections to document the network.
  - Example:
    - Summarize what the network does.
    - Include instructions or notes about inputs and outputs.
    - Include references to external assets or dependencies.

## Optimizing Performance

1. **Active Nodes Only**

- Disable nodes that aren't actively needed.

2. **Resolution Scaling**

- Set an Appropriate resolution CHOP for TOPs to avoid processing unnesseraily high resolutions.

## Modular and Reasable Design

1. **Encapsulation**

- Use Base COMPs to group related functionality. This helps in breaking down complex networks into smaller, manageable pieces.

2. **Imput/Output Clarity**

- Clearly define what goes in and out of each COMP.

3. **Reusability**

- Build a system you might reuse in the future, make it modular, paraleterized, and easy to drop into other projects.

## Project Organization

1. **Relative File Paths**

- Use relative paths instead of absolute paths to ensure the project works across different systems.

2. **Assets Folder**

- Keep all external files in a dedicated assets folder.

3. **Backups**

- Use version control or save multiple versions of your project file.

## Additional Conventions

1. **Community Conventions**

- Include a README to explain the project
- Label custom scripts and components clearly for others to understand.
- Be **Consistent**, Consistency in naming, organization, and layout will save time and effort in debugging, collaboration, and exapanding the project later.
