# LaTeX Core Templates and Themes

This repository contains core LaTeX templates and themes that can be used across different LaTeX projects, including both documents and presentations.
It includes:

- **Custom Classes:** LaTeX `.cls` files for documents (e.g., articles, reports).
- **Beamer Themes:** Custom themes for Beamer presentations.
- **Build Configuration:** Standard `.latexmkrc` and `Makefile` for consistent build processes.

## How to Use

To incorporate the resources from this repository into your LaTeX project, follow these steps:

1. **Add as a Submodule:**

   If you have an existing Git project, you can add this repository as a submodule:
   ```bash
   git submodule add https://github.com/yourusername/latex-core.git assets/core
   ```

   This will include the latex-core repository within the assets/core directory of your project.

2. **Include the Classes and Themes:**

   In your LaTeX document or presentation, you can include the classes or themes by referencing the paths to these files.
   For example, in a document:

   ```latex
   \documentclass{assets/core/classes/customdoc}
   ```

   For Beamer presentations:

   ```latex
   \documentclass{beamer}
   \usetheme{assets/core/themes/slides/slidetheme}
   ```

3. Build Your Project:

   Use the provided .latexmkrc and Makefile to compile your LaTeX documents.
   The build process will automatically use the resources from this repository.


## Customization

You can customize the LaTeX classes and themes provided in this repository to fit your specific needs.
Simply edit the .cls files or theme files within the classes/ or themes/ directories.

### Example Custom Class

Here's an example of a minimal custom LaTeX class:

```latex
\NeedsTeXFormat{LaTeX2e}
\ProvidesClass{customdoc}[2024/08/22 Custom Document Class]

\LoadClass{article} % Base class

% Customizations go here
```

### Example Beamer Theme

Here's an example of a minimal Beamer theme:

```latex
\ProvidesPackage{beamerthemeCustom}

\mode<presentation>
{
    % Customizations go here
    \setbeamercolor{title}{fg=white,bg=red}
}
```

## Contributing

Contributions to this repository are welcome!
If you have ideas for improving the templates, adding new themes, or making the build process more efficient, feel free to fork the repository and submit a pull request.

### Reporting Issues

If you encounter any issues or have questions about how to use the templates and themes, please open an issue on the repository.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

### What’s Included

- **Repository Structure:** A detailed breakdown of the repository's contents.
- **Usage Instructions:** Step-by-step instructions on how to add the repository as a submodule, use the classes and themes, and build your LaTeX projects.
- **Customization:** Basic examples of how to customize LaTeX classes and Beamer themes.
- **Contributing:** Guidelines for contributing to the repository and reporting issues.
repository and customize it for their own needs.
