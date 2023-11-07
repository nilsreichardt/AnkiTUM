# AnkiTUM

## Overview
AnkiTUM is a collaborative repository for computer science students at the Technical University of Munich to create and share flashcards for various CS modules. The flashcards are generated from markdown files, making it easy to contribute and maintain the content.

Please note that AnkiTUM is in its early stages.

### Downloading
Prebuilt flashcard packages (apkg files) are available on my HTTP [mirror](https://mirror.hugomelder.com/anki-decks/), and are updated automatically.

### Installation
To install the prebuilt flashcard packages:

1. Navigate to the "Actions" tab of this GitHub repository.
2. Click on the latest successful workflow run.
3. Scroll down to the "Artifacts" section.
4. Download the artifact and unpack it. You will find compressed tarballs of all available modules
5. Extract the `.apkg` files from the `.tar.gz` file.
6. Import the `.apkg` file into your Anki application.

### Updating Flashcards
When new flashcards are added or existing ones are updated, simply download the latest artifact and import it into Anki. Anki is designed to manage updates efficiently, meaning your progress with the cards, including study stats and scheduling, will not be lost when you update a deck with a newly downloaded package.

## Generating Flashcards Locally
To generate flashcards on your local machine, you need to have Python installed. Follow these steps:

1. Clone the AnkiTUM repository.
2. Navigate to the cloned directory.
3. Create a virtual environment: `python -m venv ankitum-env`
4. Activate the virtual environment:
   - On macOS and Linux: `source ankitum-env/bin/activate`
5. Install the required tool: `pip install markdown-anki-decks`
6. Run `make`. This will create `build/` with all the resulting decks

## Flashcard Format
The flashcards are structured in the markdown files as follows:

- `#`: Use the h1 tag for the deck title.
- `##`: Use h2 tags to denote questions.
- Content between h2 tags is considered the answer to the preceding question.

Maintain this format to ensure proper flashcard generation.

## Releases

Modules are released when they reach a stable iteration, reflecting the latest contributions at that time.

## Contributing

### Guidelines
We welcome contributions from TUM students to enhance and expand the AnkiTUM flashcard collection. To contribute, follow these guidelines:

1. **Create Your Flashcards:** Add or edit markdown files following the specified format for decks (h1 tags) and cards (h2 tags and content).
2. **Test Locally:** Generate the flashcards locally using the provided instructions to ensure they are formatted correctly.
3. **Commit Your Changes:** Once you've tested your flashcards, commit the changes to your forked repository.
4. **Submit a Pull Request (PR):** Create a PR against the main AnkiTUM repository. Include a clear description of your changes and any other relevant information.
5. **Review:** Wait for a repository maintainer to review your PR. Be responsive to any feedback or required changes.

### Best Practices
- Ensure your flashcards are accurate and relevant to the CS modules.
- Check for duplicates to avoid redundant content.
- Keep your markdown files organized by module and topic.

By following these guidelines, you'll help maintain the quality and usefulness of the AnkiTUM flashcard repository for all students. Your contributions are greatly appreciated!
