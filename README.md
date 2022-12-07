# Celestial

![Build Status](https://github.com/StrixzIV/Celestial/actions/workflows/test-and-lint.yml/badge.svg)

Celestial, an NLP-based Discord chatbot that can talk with you in English and Thai.

This project uses **[LST20 Corpus](https://huggingface.co/datasets/lst20)** dataset from NECTEC as a base for the chat processing module.

The full documentation of the corpus is available **[here](https://arxiv.org/pdf/2008.05055.pdf)** for more details.

Invite our bot **[here](https://discord.com/api/oauth2/authorize?client_id=927573556961869825&permissions=283669424144&scope=bot)**.

## Usage

You can talk to the bot by DM the bot or invite the bot to your server and type

```txt
<usr> your message goes here
```

to send your message to the bot.

### Examples

![Preview](./assets/Preview.png)

## Dependencies & Tools

This project requires Python 3.9 or higher.
This project uses **[Nextcord](https://github.com/nextcord/nextcord)** as Discord API wrapper and **[PyThaiNLP](https://github.com/PyThaiNLP/pythainlp)** for word tokenizing.

A list of dependencies can be found **[here](./requirements.txt)**.

You can install dependencies for development by running:

```sh
pip install -r requirements.txt
```

## Testing & Debugging

You can test the outcome of your intents by running the interactive intents tester from **[this](./cli_tester.py)** file.

This testing file shows the tokenized input messages and how the bot is responding back to you in command-line interface.

```sh
python cli_tester.py
```

### Intents tester examples

![command-line tester](./assets/cli-test-preview.png)

### Unit testing

This project uses PyTest for testing.

You can update the test case by editing files in the **[tests](./tests/)** directory.

To run the unit testing, use the command:

```sh
pytest
```

## Contributions

You can contribute by creating new intents and responses for the chatbot by simply updating the intent JSON files in **[responses](./responses)** folder (Please take a look at **[Chat Intent Development Manual](./docs/chat_intents_guide.md)**).

You can also suggest new features or improvements to the existing code by creating **[Feature request issue](https://github.com/StrixzIV/Celestial/issues/new?assignees=StrixzIV&labels=enhancement%2C+Feature+request&template=feature_request.md&title=Request%3A+)**.

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Make sure to read our code of conduct **[here](./CODE_OF_CONDUCT.md)** before starting to contribute to our project.

Please make sure to update the tests as appropriate.

## License

* **[MIT License](./LICENSE)**
