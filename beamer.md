
# Beamer – Creating Presentations Using LaTeX

## 1. Introduction

Beamer is a LaTeX document class used to create presentations and slides. It allows users to prepare professional presentations using LaTeX commands.

Unlike traditional presentation software, Beamer uses code to define slide content, formatting, themes and layouts.

### Uses of Beamer

- Creating academic presentations.
- Preparing research presentations.
- Presenting mathematical equations.
- Creating technical and educational slides.
- Preparing conference presentations.

## 2. Basic Structure of a Beamer Presentation

A Beamer presentation starts with the `beamer` document class.

### Example

```latex
\documentclass{beamer}

\title{Introduction to Computer Science}
\author{Student Name}
\institute{College Name}
\date{\today}

\begin{document}

\begin{frame}
    \titlepage
\end{frame}

\begin{frame}{Introduction}
    Welcome to my presentation.
\end{frame}

\end{document}
```

### Explanation

- `\documentclass{beamer}` selects the Beamer class.
- `\title` defines the presentation title.
- `\author` specifies the presenter.
- `\institute` specifies the institution.
- `\date` defines the presentation date.
- `\begin{frame}` starts a new slide.
- `\titlepage` displays the title slide.
- `\end{frame}` ends the current slide.

## 3. Creating Slides Using Frames

In Beamer, each slide is called a frame.

The `frame` environment is used to create individual slides.

### Example

```latex
\begin{frame}{Introduction}
    Beamer is used to create presentations.

    It provides different themes and layouts.
\end{frame}

\begin{frame}{Features}
    Beamer supports:
    \begin{itemize}
        \item Mathematical equations
        \item Images
        \item Tables
        \item Animations
    \end{itemize}
\end{frame}
```

Each frame creates a separate slide in the presentation.

## 4. Themes and Color Themes

Beamer provides built-in themes that control the overall appearance of a presentation.

### Applying a Theme

```latex
\usetheme{Madrid}
```

Some commonly used themes are:

| Theme | Description |
|---|---|
| Madrid | Clean and structured layout |
| Berlin | Navigation-oriented layout |
| CambridgeUS | Traditional academic appearance |
| Copenhagen | Structured presentation style |
| Warsaw | Formal presentation layout |
| Singapore | Minimal presentation style |

### Changing Color Themes

Color themes control the colors used in a presentation.

```latex
\usecolortheme{beaver}
```

Other examples include:

- dolphin
- seahorse
- whale
- orchid

## 5. Adding Lists and Bullet Points

Beamer supports the same list environments used in LaTeX.

### Unordered List

```latex
\begin{frame}{Advantages}
    \begin{itemize}
        \item Easy formatting
        \item Professional slides
        \item Mathematical support
    \end{itemize}
\end{frame}
```

### Ordered List

```latex
\begin{frame}{Steps}
    \begin{enumerate}
        \item Create a document.
        \item Add presentation content.
        \item Compile the presentation.
    \end{enumerate}
\end{frame}
```

## 6. Adding Images to Slides

The `graphicx` package is used to insert images into Beamer presentations.

### Example

```latex
\usepackage{graphicx}

\begin{frame}{System Architecture}
    \centering
    \includegraphics[width=0.7\textwidth]{diagram.png}
\end{frame}
```

The image is displayed in the slide with center alignment.

## 7. Creating Columns

Beamer supports multiple columns within a single frame.

This is useful when displaying text and images side by side.

### Example

```latex
\begin{frame}{Two Column Layout}

\begin{columns}

\column{0.5\textwidth}
Left Column

\column{0.5\textwidth}
Right Column

\end{columns}

\end{frame}
```

The `columns` environment divides a slide into multiple sections.

## 8. Adding Mathematical Equations

Beamer supports mathematical expressions using standard LaTeX syntax.

### Example

```latex
\begin{frame}{Mathematical Equation}

\[
E = mc^2
\]

\[
a^2 + b^2 = c^2
\]

\end{frame}
```

This makes Beamer useful for scientific and engineering presentations.

## 9. Overlays and Step-by-Step Content

Beamer provides overlay commands that reveal presentation content in stages.

### Using Pause

```latex
\begin{frame}{Learning Objectives}

\begin{itemize}
    \item Understand LaTeX.
    \pause
    \item Learn Beamer.
    \pause
    \item Create presentations.
\end{itemize}

\end{frame}
```

The `\pause` command reveals content progressively across presentation steps.

### Using Item Specifications

```latex
\begin{itemize}
    \item<1-> Introduction
    \item<2-> Main Content
    \item<3-> Conclusion
\end{itemize}
```

The `<1->`, `<2->` and `<3->` specifications control when individual items appear.

## 10. Compiling a Beamer Presentation

The general workflow is:

1. Create a `.tex` file.
2. Select the Beamer document class.
3. Define the title and author.
4. Add frames containing slide content.
5. Apply a suitable theme.
6. Compile the file using a LaTeX distribution or online editor.
7. Review the generated PDF presentation.

### Common Tools

- Overleaf
- TeX Live
- MiKTeX

## 11. Advantages of Beamer

- Produces professionally formatted presentations.
- Supports mathematical equations.
- Provides reusable themes.
- Supports images, tables and columns.
- Allows step-by-step content presentation.
- Integrates with the LaTeX ecosystem.

## 12. What I Learned

Through Beamer, I learned how to create presentations using LaTeX commands.

I understood how to create frames, apply themes, insert images, organize content into columns and display information progressively.

Beamer is useful for academic and technical presentations because it provides structured formatting and consistent slide design.
