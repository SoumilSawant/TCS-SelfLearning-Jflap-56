# Theory of Computer Science: Self-Learning with JFLAP

- **Name:** Soumil Mahesh Sawant
- **Roll No.:** 56
- **Class / Branch / Sem:** D12B / CMPN / Semester V
- **Subject:** Theory of Computer Science (26CMPC51)

This repository contains 30 JFLAP (`.jff`) examples covering finite automata, transducers, regular expressions, regular and context-free grammars, LL/LR/CYK parsing, pushdown automata, Turing machines, and Chomsky Normal Form transformations.

## Setup & Usage

1. Ensure Java (JDK/JRE 8+) is installed on your machine.
2. Download JFLAP 7.1 from https://www.jflap.org/modules/.
3. Launch JFLAP and open any `.jff` file via **File → Open**.

## List of JFLAP Files

| #   | Topic                                      | File                                                            | Description                                                                |
| --- | ------------------------------------------ | --------------------------------------------------------------- | -------------------------------------------------------------------------- | ---------------------------------------------------- | ------------------------------------ |
| 1   | Deterministic Finite Automata              | `56_SoumilSawant_deterministic_finite_automata_18-11-26.jff`    | DFA over {0,1} accepting strings that end in "01"                          |
| 2   | Nondeterministic Finite Automata           | `56_SoumilSawant_nondeterministic_finite_automata_18-11-26.jff` | NFA over {a,b} accepting strings starting and ending with "b"              |
| 3   | NFA to DFA Conversion                      | `56_SoumilSawant_nfa_to_dfa_conversion_18-11-26.jff`            | NFA over {0,1} for strings whose third-from-last symbol is "1"             |
| 4   | DFA Minimization                           | `56_SoumilSawant_dfa_minimization_18-11-26.jff`                 | 4-state DFA over {a,b} for even-length strings that minimizes to 2 states  |
| 5   | DFA to Regular Grammar Conversion          | `56_SoumilSawant_dfa_to_regular_grammar_18-11-26.jff`           | DFA accepting strings over {a,b} with an odd number of b's                 |
| 6   | DFA to Regular Expression Conversion       | `56_SoumilSawant_dfa_to_regular_expression_18-11-26.jff`        | DFA accepting strings over {0,1} ending with "00"                          |
| 7   | Combining Automata                         | `56_SoumilSawant_combining_automata_18-11-26.jff`               | DFA for strings over {a,b} containing "bb", for union or concatenation     |
| 8   | Regular Expression                         | `56_SoumilSawant_regular_expression_18-11-26.jff`               | Regular expression (0+1)\*010                                              |
| 9   | Regular Expression to DFA Conversion       | `56_SoumilSawant_regex_to_dfa_18-11-26.jff`                     | Regular expression (a+b)\*aba for conversion to DFA                        |
| 10  | Regular Expression Identities              | `56_SoumilSawant_regular_expression_identities_18-11-26.jff`    | Regular expression (a*b*)_ for verifying equivalence with (a+b)_           |
| 11  | Regular Grammar                            | `56_SoumilSawant_regular_grammar_18-11-26.jff`                  | Right-linear regular grammar generating b\*ab                              |
| 12  | Regular Grammar to DFA Conversion          | `56_SoumilSawant_regular_grammar_to_dfa_18-11-26.jff`           | Right-linear grammar for strings starting with a and ending with b         |
| 13  | DFA Relationship to Grep                   | `56_SoumilSawant_dfa_grep_110_18-11-26.jff`                     | DFA for (0+1)\*110 demonstrating grep substring pattern matching           |
| 14  | Mealy Machine                              | `56_SoumilSawant_mealy_1s_complement_18-11-26.jff`              | Mealy machine that computes the 1's complement of a binary string          |
| 15  | Moore Machine                              | `56_SoumilSawant_moore_detect_10_18-11-26.jff`                  | Moore machine that outputs 1 right after "10" is seen                      |
| 16  | Context-free Grammar                       | `56_SoumilSawant_context_free_grammar_18-11-26.jff`             | CFG S -> aSbb                                                              | lambda generating a^n b^(2n)                         |
| 17  | Pushdown Automata                          | `56_SoumilSawant_pushdown_automaton_18-11-26.jff`               | NPDA accepting odd-length palindromes with center marker c (w c w^R)       |
| 18  | NPDA to CFG Conversion                     | `56_SoumilSawant_npda_to_cfg_conversion_18-11-26.jff`           | NPDA for a^n b^n (n >= 1) formatted for direct CFG conversion              |
| 19  | CFG to NPDA Conversion                     | `56_SoumilSawant_cfg_to_npda_conversion_18-11-26.jff`           | CFG for even-length palindromes over {a,b} to convert into an NPDA         |
| 20  | Context-free Grammar with Single Symbols   | `56_SoumilSawant_cfg_single_symbols_18-11-26.jff`               | CFG whose right-hand sides are single terminal or non-terminal symbols     |
| 21  | Context-free Grammar with Multiple Symbols | `56_SoumilSawant_cfg_multiple_symbols_18-11-26.jff`             | CFG with multi-symbol right-hand sides (S -> aBCd)                         |
| 22  | CFG in Error using User Control Parse      | `56_SoumilSawant_cfg_error_parse_18-11-26.jff`                  | CFG S -> aSa                                                               | ba for demonstrating dead-ends in User Control Parse |
| 23  | LL Parsing                                 | `56_SoumilSawant_ll_parsing_18-11-26.jff`                       | LL(1) grammar for balanced parentheses expressions S -> (S)S               | lambda                                               |
| 24  | LR Parsing                                 | `56_SoumilSawant_lr_parsing_18-11-26.jff`                       | LR(1) grammar E -> E\*T                                                    | T, T -> (E)                                          | a for bottom-up shift-reduce parsing |
| 25  | CYK Parsing                                | `56_SoumilSawant_cyk_parsing_18-11-26.jff`                      | Grammar in Chomsky Normal Form generating a^n b^n (n >= 1) for CYK parsing |
| 26  | One-Tape Turing Machine                    | `56_SoumilSawant_one_tape_turing_machine_18-11-26.jff`          | One-tape TM that inverts binary strings (replaces 0 with 1 and 1 with 0)   |
| 27  | Multi-Tape Turing Machine                  | `56_SoumilSawant_multi_tape_turing_machine_18-11-26.jff`        | Two-tape TM that recognizes a^n b^n (n >= 1) using the second tape         |
| 28  | Turing Machine Building Blocks             | `56_SoumilSawant_turing_building_block_18-11-26.jff`            | TM building block subroutine that moves left to the first blank symbol     |
| 29  | Unrestricted Grammar                       | `56_SoumilSawant_unrestricted_grammar_18-11-26.jff`             | Type-0 unrestricted grammar that generates a^n b^n c^n (n >= 1)            |
| 30  | CFG to Chomsky Normal Form Transformation  | `56_SoumilSawant_cfg_to_cnf_transformation_18-11-26.jff`        | CFG with lambda, unit, and mixed productions for CNF transformation        |
