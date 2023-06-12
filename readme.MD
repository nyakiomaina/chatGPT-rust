# OpenAI SQL Code Generator in Rust
Simple Rust program that uses the OpenAI API to generate SQL code based on user input.

## About
This application takes user input from the console, which should be a natural language statement, and sends it to the OpenAI API, which generates a corresponding SQL query based on the input. It uses the "text-davinci-001" engine for text generation.

The user input is appended to a static preamble: "Generate a Sql code for the given statement". The response from the API, which is a SQL query, is then printed to the console. The program runs in a loop, allowing the user to provide input and receive SQL queries continuously.

## Prerequisites
Rust Programming Language
OpenAI account and API key
hyper, hyper-tls, dotenv, serde, serde_derive, spinners crates

## Installation
Before you can run this program, you need to have Rust installed on your machine. If you don't have Rust installed, follow the instructions [here] (https://www.rust-lang.org/tools/install) to install it.

You also need an API key from OpenAI. If you don't have one, you can create an account on the [OpenAIwebsite] (https://openai.com/) , then follow the instructions to get an API key.

Add the following to your Cargo.toml file:

```bash

[dependencies]
hyper = "*"
hyper-tls = "*"
dotenv = "*"
serde = "*"
serde_derive = "*"
spinners = "*"
```

## Usage
First, create a .env file in the root of your project and add the following line to it:

```bash

OAI_TOKEN=<Your OpenAI API Key>
```

Remember to replace <Your OpenAI API Key> with your actual OpenAI API key.

Then, you can run the program with the following command:

```bash
cargo run
```

You will be prompted to enter a statement in natural language. After you do, press Enter, and the application will display the corresponding SQL query.

## Contributing

Contributions, issues and feature requests are welcome.