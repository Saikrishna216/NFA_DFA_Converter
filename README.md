# NFA to DFA Converter

The **NFA to DFA Converter** is a web-based tool designed to help users convert a Non-deterministic Finite Automaton (NFA) into its equivalent Deterministic Finite Automaton (DFA). The application provides an intuitive user interface for defining NFA states, transitions (including epsilon transitions), and final states. Once the NFA is defined, the converter uses standard automata theory algorithms to compute the corresponding DFA. 

The results are then displayed in two formats:
- **DFA Transition Table:** A tabular view of the DFA transitions, highlighting the start state and final states.
- **DFA Graph:** An interactive, dark-themed graph visualization rendered using the [vis-network](https://visjs.github.io/vis-network/) library. This graph features advanced edge separation techniques to handle overlapping transitions and a fixed layout so that the nodes remain in place.

The entire website is designed with a dark theme, ensuring a modern, sleek look with cohesive styling across all components—from input forms and tables to the interactive graph.

## Features

- **State and Transition Input:**  
  - Easily add and remove states.
  - Define transitions by selecting source and target states along with the input symbol (ε for epsilon transitions).
  - Toggle a state as final by clicking it, and set a start state by double-clicking on it.

- **NFA to DFA Conversion:**  
  - Implements the standard conversion algorithm using epsilon closures and state moves.
  - Automatically computes and displays the DFA, including the transition table and graph.

- **Visual Output:**  
  - **DFA Transition Table:**  
    Clearly displays each DFA state along with transitions for every input symbol, and marks the start and final states.
  - **DFA Graph:**  
    An interactive graph view of the DFA with separated overlapping edges and a fixed layout for better clarity.

- **Dark Theme:**  
  The entire application uses a cohesive dark theme, with global styling ensuring dark backgrounds, light text, and carefully chosen accent colors.

- **Data Export:**  
  Users can export the complete conversion (including both the NFA and DFA data) as a JSON file for further analysis or documentation.

## Technologies Used

- **React** – Front-end library for building the user interface.
- **TypeScript** – Adds type safety and robust error checking.
- **Tailwind CSS** – Provides a utility-first approach for styling and theming.
- **vis-network** – Offers advanced interactive graph visualization.
- **Dagre** – Used for potential layout calculations.
  
## Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/Saikrishna216/nfa-dfa-converter.git
   cd nfa-dfa-converter
