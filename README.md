# LangChainGo Chat Example

This repository contains an example Go application that demonstrates the use of the `langchaingo` package to interact with a language model for chat purposes. The main functionality is to send messages to the language model and receive responses, which could be used for generating creative content, answering questions, or other language-based tasks.

## Prerequisites

Before you can run this example, you need to ensure you have the following prerequisites installed:

- Go (version 1.15 or later)
- Access to the `langchaingo` package and its dependencies

## Installation

To use this example, you need to install the `langchaingo` package along with its dependencies. You can do this by running:

```sh
go get github.com/tmc/langchaingo/llms
go get github.com/tmc/langchaingo/llms/ollama
go get github.com/tmc/langchaingo/schema
```

## Usage

The main.go file contains the entry point for the application. It sets up a new chat with the language model and sends a series of messages to it. The responses are then printed to the standard output.

To run the example, navigate to the directory containing main.go and execute:

```
go run main.go
```

## Code Explanation

The code performs the following steps:

- Initializes a new chat session with the language model using the ollama.- - NewChat function, specifying the model name as "llama2".
- Creates a context for handling cancellation and timeouts.
- Sends a system message to the language model instructing it to provide precise answers without verbosity.
- Sends a human message asking for creative company names for a colorful sock company and requests three examples.
- Sets up a streaming function to print the language model's responses as they are received.
- Prints the final completion message received from the language model.

## Contributing

If you'd like to contribute to this project, please feel free to submit pull requests or open issues to discuss potential changes or improvements.

License
This example is provided under the MIT License. See the LICENSE file for more details.

## Disclaimer

This example is for demonstration purposes only and is not intended for production use. The langchaingo package and its dependencies are external resources and their usage is subject to their respective licenses and terms of service.

This README provides a basic overview of the example Go application, its prerequisites, installation steps, usage instructions, a brief code explanation, contribution guidelines, licensing information, and a disclaimer. Adjust the content as necessary to match the actual details of your repository and the `langchaingo` package.
