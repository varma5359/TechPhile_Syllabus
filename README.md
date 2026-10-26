# MASTER PROMPT: Generate 29,700 Unique MCQs for TechPhile.ai

## 1. Role

Act as a Senior Technical Assessment Architect, Subject Matter Expert, Technical Interviewer, Curriculum Designer, and Python Data Quality Engineer.

Generate a complete, professional question bank for TechPhile.ai covering 33 technical and aptitude categories. The question bank must support students, freshers, job seekers, and working professionals preparing for assessments and interviews.

Every question must be technically correct, unique, unambiguous, relevant to its category, and appropriate for its assigned difficulty level.

## 2. Project context

- Repository: `D:\TechPhile_first_version\techphile_exams`
- Output folder: `techphile_question_bank`
- Output format: UTF-8 CSV
- Questions per category per difficulty level: 300
- Sets per CSV file: 10
- Questions per set: 30
- Difficulty levels: Beginner, Intermediate, Advanced
- CSV files per category: 3
- Total categories: 33
- Total CSV files: 99
- Total questions: 29,700

**Critical requirement:** Each CSV file must contain exactly 300 questions, not 100. Do not confuse the number of questions per difficulty level with the number of questions across all difficulty levels.

## 3. Exact output structure

Create one folder containing 99 CSV files, organized into one subfolder per category.

Example:

```text
techphile_question_bank/
├── Python/
│   ├── python_beginner.csv
│   ├── python_intermediate.csv
│   └── python_advanced.csv
├── Java/
│   ├── java_beginner.csv
│   ├── java_intermediate.csv
│   └── java_advanced.csv
├── JavaScript/
│   ├── javascript_beginner.csv
│   ├── javascript_intermediate.csv
│   └── javascript_advanced.csv
└── ...remaining 30 categories
```

Use lowercase filenames and underscores. Keep category folder names consistent with the canonical category names.

### Example: Python

**File 1: `python_beginner.csv`**
- Exactly 300 Beginner questions.
- Set 1: questions 1–30.
- Set 2: questions 31–60.
- Set 3: questions 61–90.
- Set 4: questions 91–120.
- Set 5: questions 121–150.
- Set 6: questions 151–180.
- Set 7: questions 181–210.
- Set 8: questions 211–240.
- Set 9: questions 241–270.
- Set 10: questions 271–300.

**File 2: `python_intermediate.csv`**
- Exactly 300 Intermediate questions.
- Set 1 through Set 10, with 30 questions per set.

**File 3: `python_advanced.csv`**
- Exactly 300 Advanced questions.
- Set 1 through Set 10, with 30 questions per set.

Apply the same structure to all 33 categories.

## 4. The 33 mandatory categories

Generate separate Beginner, Intermediate, and Advanced CSV files for every category listed below.

1. Python
2. Java
3. JavaScript
4. C
5. C++
6. SQL
7. HTML
8. CSS
9. React
10. Django
11. Flask
12. FastAPI
13. NumPy
14. Pandas
15. Matplotlib
16. Seaborn
17. Scikit-learn
18. Statistics
19. Excel
20. Power BI
21. Machine Learning
22. Deep Learning
23. Artificial Intelligence
24. Generative AI
25. NLP
26. Computer Vision
27. Git and GitHub
28. Data Structures and Algorithms
29. Spring Boot
30. REST APIs
31. MongoDB
32. MySQL
33. Aptitude

Do not omit, merge, rename, or replace any category.

## 5. Exact quantity rules

For every category:

| Difficulty | CSV files | Questions per file | Sets per file |
|---|---:|---:|---:|
| Beginner | 1 | 300 | 10 |
| Intermediate | 1 | 300 | 10 |
| Advanced | 1 | 300 | 10 |
| **Total per category** | **3** | **900** | **30** |

For the complete question bank:

- 33 categories
- 3 difficulty levels per category
- 99 CSV files
- 300 questions per file
- 10 sets per file
- 30 questions per set
- 990 sets in total
- **29,700 questions in total**

Do not produce fewer questions, placeholder rows, empty questions, or duplicate rows to meet the required count.

## 6. Difficulty-level rules

Each CSV file must contain only its assigned difficulty level.

### Beginner CSV

Generate 300 beginner-level questions covering foundational concepts, syntax, terminology, basic operations, simple examples, straightforward code interpretation, and common introductory mistakes.

Questions must be accessible to learners who have recently started the subject.

### Intermediate CSV

Generate 300 intermediate-level questions covering practical application, multi-step reasoning, debugging, realistic scenarios, combining related concepts, and interpreting code, queries, formulas, or outputs.

Questions should assume a reasonable understanding of the subject's fundamentals.

### Advanced CSV

Generate 300 advanced-level questions covering complex scenarios, edge cases, deeper reasoning, optimization, performance, trade-offs, architecture, and advanced applications where relevant to the category.

Questions must be challenging because of the reasoning or technical knowledge required, not because the wording is confusing.

### Mandatory difficulty validation

- `python_beginner.csv` must contain exactly 300 Beginner questions.
- `python_intermediate.csv` must contain exactly 300 Intermediate questions.
- `python_advanced.csv` must contain exactly 300 Advanced questions.
- Apply the same rule to all other categories.
- Never mix difficulty levels inside a CSV file.

## 7. Set rules

Each CSV file must contain exactly 10 sets, with 30 questions in every set.

| Set | Question numbers | Count |
|---|---|---:|
| Set 1 | 1–30 | 30 |
| Set 2 | 31–60 | 30 |
| Set 3 | 61–90 | 30 |
| Set 4 | 91–120 | 30 |
| Set 5 | 121–150 | 30 |
| Set 6 | 151–180 | 30 |
| Set 7 | 181–210 | 30 |
| Set 8 | 211–240 | 30 |
| Set 9 | 241–270 | 30 |
| Set 10 | 271–300 | 30 |
| **Total** | **1–300** | **300** |

Rules:

1. Every set must contain exactly 30 questions.
2. `question_number` must be sequential from 1 through 300 within each file.
3. `set_number` must be an integer from 1 through 10.
4. `set_name` must use `Set 01` through `Set 10`.
5. Every question must belong to exactly one set.
6. Question numbering restarts at 1 for every CSV file.
7. The last set must contain questions 271–300, not a partial set.

## 8. Required CSV schema

Use these exact columns in this order:

1. `question_id`
2. `category`
3. `difficulty`
4. `set_number`
5. `set_name`
6. `question_number`
7. `topic`
8. `subtopic`
9. `question_type`
10. `question`
11. `option_a`
12. `option_b`
13. `option_c`
14. `option_d`
15. `correct_option`
16. `correct_answer`
17. `explanation`
18. `learning_objective`
19. `tags`

### Column requirements

- `question_id`: Globally unique identifier across all 99 files.
- `category`: Exact canonical category name.
- `difficulty`: Exactly `Beginner`, `Intermediate`, or `Advanced`.
- `set_number`: Integer from 1 through 10.
- `set_name`: `Set 01` through `Set 10`.
- `question_number`: Integer from 1 through 300 within each file.
- `topic`: Main concept assessed.
- `subtopic`: Specific concept or skill.
- `question_type`: Appropriate question type, such as `Conceptual`, `Code Output`, `Debugging`, `Scenario`, `Application`, `Query`, `Calculation`, or `Algorithm`.
- `question`: Complete, clear question text.
- `option_a` to `option_d`: Four distinct answer options.
- `correct_option`: Exactly one of `A`, `B`, `C`, or `D`.
- `correct_answer`: Exact text of the correct option.
- `explanation`: Explanation supporting the correct answer.
- `learning_objective`: The concept or skill the learner should demonstrate.
- `tags`: Relevant keywords separated by semicolons.

Do not leave required fields empty. Use valid CSV escaping for commas, quotation marks, and multiline text. Prefer single-line question, option, and explanation fields for easier importing.

## 9. Four-option MCQ rules

Every question must have exactly four answer options.

1. Exactly one option must be correct.
2. All options must be relevant to the question.
3. Distractors must be plausible and educationally useful.
4. Options must not be duplicates or trivial wording variations.
5. Avoid “All of the above” and “None of the above.”
6. Avoid grammatical clues that reveal the correct answer.
7. Avoid making the correct answer consistently longer or more detailed.
8. Distribute correct answer letters across A, B, C, and D without an obvious repeating pattern.
9. Never change a correct answer merely to balance answer-letter distribution.
10. Ensure the `correct_answer` text exactly matches the option identified by `correct_option`.

## 10. Question uniqueness rules

Uniqueness is mandatory across the **entire collection of 29,700 questions**, not merely within individual CSV files.

Do not duplicate questions:

- Within the same set.
- Across sets in the same file.
- Across different difficulty levels of the same category.
- Across different categories.
- By changing only variable names, numbers, option order, or superficial wording.

Questions may assess related concepts, but they must test materially different learning objectives or reasoning.

For example, changing `x = 5` to `x = 10` in an otherwise identical Python question does not make it a genuinely unique question.

Implement duplicate detection using normalized question text and semantic review. Automated text comparison is useful but is not sufficient to establish semantic uniqueness.

If duplicates are found, replace them with distinct questions and revalidate the affected files.

## 11. Explanation and answer rules

Every question must have a useful explanation.

The explanation must:

- Explain why the correct answer is correct.
- Show the relevant reasoning, rule, or calculation.
- Clarify a key distinction or misconception when useful.
- Match the stated assumptions and the correct option.
- Avoid unsupported claims and unrelated background information.

For code, query, formula, calculation, and algorithm questions, independently verify the result.

Do not fabricate APIs, syntax, outputs, statistics, or technical behavior.

Where version differences matter, state the relevant version or assumptions in the question or explanation.

## 12. Category-specific content rules

Build a distinct, appropriate topic distribution for every category and difficulty level.

### Programming languages

For Python, Java, JavaScript, C, and C++, cover fundamentals, data types, operators, control flow, functions, collections or data structures, debugging, error handling, language-specific behavior, and advanced concepts as appropriate.

### Databases and SQL

For SQL, MySQL, and MongoDB, cover queries, filtering, aggregation, joins or document relationships where applicable, indexing, constraints, data modeling, transactions, performance, and practical data scenarios.

Keep general SQL and MySQL-specific syntax distinct. Do not apply relational database concepts incorrectly to MongoDB.

### Web technologies and frameworks

For HTML, CSS, React, Django, Flask, FastAPI, Spring Boot, and REST APIs, cover their actual syntax, architecture, request processing, data handling, validation, security, testing, error handling, and practical use cases.

Do not mix features from different frameworks or rely on obsolete APIs without identifying the relevant context.

### Data analysis and visualization

For NumPy, Pandas, Matplotlib, Seaborn, Excel, and Power BI, cover data operations, transformations, formulas, aggregation, visualization, interpretation, and practical business scenarios.

### Statistics, ML, and AI

For Statistics, Scikit-learn, Machine Learning, Deep Learning, Artificial Intelligence, Generative AI, NLP, and Computer Vision, cover foundations, algorithms, assumptions, model training, evaluation, practical applications, limitations, and appropriate advanced topics.

Include model evaluation, overfitting, generalization, data leakage, preprocessing, and model selection where relevant. Do not imply that one model or metric is best for every problem.

### Git and GitHub

Cover repository fundamentals, commits, branching, merging, pull requests, conflicts, collaboration, troubleshooting, and advanced workflows.

### Data Structures and Algorithms

Cover complexity, arrays, strings, linked lists, stacks, queues, trees, graphs, searching, sorting, recursion, hashing, and algorithmic reasoning at appropriate difficulty levels.

### Aptitude

Cover numerical ability, percentages, ratios, averages, profit and loss, time and work, speed and distance, probability, permutations and combinations, logical reasoning, sequences, and other relevant assessment topics.

Ensure every calculation question has been checked independently.

## 13. Quality rules

Before saving a question, verify:

- The question is understandable and unambiguous.
- It tests the intended topic and learning objective.
- It belongs to the correct category and difficulty.
- The four options are distinct and plausible.
- Exactly one answer is correct.
- The answer text matches the correct option.
- The explanation is accurate.
- The question is not a duplicate.
- Any code, SQL, formula, or calculation has been checked.
- The question is useful for an assessment or interview.

Do not fill quotas with meaningless variations, repetitive definitions, trivial distractors, or questions that test the same idea repeatedly.

## 14. Generation strategy

Generate the question bank systematically.

### Phase 1: Inspect

Inspect the repository, destination, existing schemas, and category definitions. Protect existing files and user changes.

### Phase 2: Plan

For every category, create a topic coverage plan for Beginner, Intermediate, and Advanced levels. Allocate topics across 10 sets so that each level has broad coverage and minimal repetition.

Do not use the same question template repeatedly with only names or numbers changed.

### Phase 3: Generate

Generate 300 questions for each category-level combination. Save each completed CSV to its correct category folder.

Create all 99 required files.

### Phase 4: Validate

Validate each CSV independently, then validate the full collection across all 99 files.

### Phase 5: Repair

Correct missing rows, duplicates, invalid answers, incorrect difficulty labels, broken CSV formatting, and incorrect set assignments.

Rerun the relevant checks after repairs.

### Phase 6: Report

Provide a concise completion report with:

- Output folder path.
- Number of CSV files created.
- Number of questions in each file.
- Number of sets in each file.
- Per-category totals.
- Per-difficulty totals.
- Duplicate-detection results.
- Answer and schema validation results.
- Any issues that remain unresolved.

Do not claim successful validation unless the checks actually ran and passed.

## 15. Mandatory automated validation

Create a temporary or reusable validation script if useful, without changing the TechPhile.ai application.

Run the following checks:

### File validation

- Exactly 99 expected CSV files exist.
- Every category has exactly three CSV files.
- Every CSV has the exact required columns in the specified order.
- Every CSV can be parsed without malformed rows.
- Every CSV contains exactly 300 data rows.
- Every CSV contains exactly 10 sets.
- Every set contains exactly 30 questions.

### Category and difficulty validation

- Each category has exactly 900 questions across its three files.
- Each category has exactly 300 Beginner questions.
- Each category has exactly 300 Intermediate questions.
- Each category has exactly 300 Advanced questions.
- Across all categories, there are exactly 9,900 questions at each difficulty level.
- Across all categories, there are exactly 29,700 questions.

### Identifier and sequence validation

- Every `question_id` is globally unique across all files.
- Each file's `question_number` runs sequentially from 1 through 300.
- Each set's question numbers match the expected 30-question range.
- Set numbers and names are consistent.
- Each file contains only the category and difficulty specified by its filename.

### MCQ validation

- No required field is empty.
- All four options are present and distinct.
- `correct_option` is one of A, B, C, or D.
- `correct_answer` matches the selected option exactly.
- Every explanation is present.
- No question has multiple correct answers.
- Code, query, calculation, and formula answers are verified as far as practical.

### Uniqueness validation

- No exact duplicate questions exist across the 99 files.
- Detect near-duplicate wording using normalized text comparisons.
- Review semantically similar questions and replace those that test the same thing in essentially the same way.
- Recheck uniqueness after replacement.

### Final pass criteria

The generation is complete only when all required files exist and all count, structure, set, difficulty, identifier, and answer checks pass.

If a validation cannot be performed automatically, report that limitation explicitly rather than marking it as passed.

## 16. Naming conventions

Use the following exact filename pattern:

`<category_slug>_<difficulty_slug>.csv`

Examples:

- `python_beginner.csv`
- `python_intermediate.csv`
- `python_advanced.csv`
- `javascript_beginner.csv`
- `machine_learning_intermediate.csv`
- `data_structures_and_algorithms_advanced.csv`
- `git_and_github_beginner.csv`

Use consistent, lowercase category slugs. Keep the canonical category name in the `category` column even when the filename uses a slug.

## 17. Restrictions

- Do not modify existing TechPhile.ai application code.
- Do not modify models, migrations, settings, templates, views, URLs, or databases.
- Do not install unnecessary dependencies.
- Do not overwrite existing files without approval.
- Do not delete or reset repository content.
- Do not commit, push, deploy, or publish.
- Do not create a single combined CSV instead of the required 99 files.
- Do not generate 100 questions per file; every file must contain 300.
- Do not mix difficulty levels inside a file.
- Do not generate placeholder or fabricated questions.
- Do not claim that semantic uniqueness is guaranteed by exact-text checks alone.
- Do not report success before running validation.

## 18. Final acceptance criteria

The work is accepted only when all the following are true:

1. All 33 categories are included.
2. Every category has one Beginner, one Intermediate, and one Advanced CSV.
3. There are exactly 99 CSV files.
4. Every CSV contains exactly 300 unique questions.
5. Every CSV contains exactly 10 sets of 30 questions.
6. Every CSV contains only its assigned difficulty level.
7. Every question has four options, one correct answer, and an explanation.
8. All required schema, identifier, set, answer, and quantity checks pass.
9. Duplicate questions have been checked across the complete collection and any detected duplicates have been addressed.
10. The final collection contains exactly 29,700 questions.
11. Existing repository content and user changes remain untouched.
12. A final report documents the actual validation results and output location.

**Begin by inspecting the repository and confirming the output destination. Then generate the complete question bank, validate it, repair any failures, and report the verified results.**