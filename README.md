# Dynamic BAML 🌟

![Dynamic BAML](https://img.shields.io/badge/Dynamic_BAML-Python_library-blue.svg)  
[![Releases](https://img.shields.io/badge/Releases-v1.0.0-orange.svg)](https://github.com/pixelcoweb/dynamic-baml/releases)

Dynamic BAML is a powerful Python library designed for dynamic BAML schema generation and LLM structured data extraction. Built on the robust BoundaryML framework, it provides seamless support for leading AI models, including OpenAI, Anthropic, Ollama, and OpenRouter. 

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Examples](#examples)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Features

- **Dynamic Schema Generation**: Automatically create BAML schemas based on your data needs.
- **Structured Data Extraction**: Efficiently extract structured data from various sources using LLMs.
- **Multi-Model Support**: Works with OpenAI, Anthropic, Ollama, and OpenRouter, providing flexibility in your projects.
- **Easy Integration**: Simple to integrate into existing Python projects with minimal setup.
- **Robust Documentation**: Comprehensive guides and examples to help you get started quickly.

## Installation

To install the Dynamic BAML library, use pip:

```bash
pip install dynamic-baml
```

After installation, you can verify it by running:

```bash
python -c "import dynamic_baml; print(dynamic_baml.__version__)"
```

## Usage

Dynamic BAML offers a straightforward API for generating BAML schemas and extracting structured data. Below is a simple example of how to use the library.

### Basic Example

```python
from dynamic_baml import BAMLGenerator

# Initialize the BAML generator
generator = BAMLGenerator()

# Generate a BAML schema
schema = generator.generate_schema(data_source="your_data_source")

# Output the generated schema
print(schema)
```

### Structured Data Extraction

You can also use Dynamic BAML to extract structured data using your preferred LLM model.

```python
from dynamic_baml import DataExtractor

# Initialize the data extractor
extractor = DataExtractor(model="openai")

# Extract structured data
structured_data = extractor.extract(data="your_raw_data")

# Output the structured data
print(structured_data)
```

## Examples

### Example 1: Generating a BAML Schema

```python
from dynamic_baml import BAMLGenerator

data_source = {
    "name": "John Doe",
    "age": 30,
    "occupation": "Software Developer"
}

generator = BAMLGenerator()
schema = generator.generate_schema(data_source=data_source)

print("Generated BAML Schema:")
print(schema)
```

### Example 2: Extracting Structured Data

```python
from dynamic_baml import DataExtractor

raw_data = "John Doe is a 30-year-old Software Developer."

extractor = DataExtractor(model="anthropic")
structured_data = extractor.extract(data=raw_data)

print("Extracted Structured Data:")
print(structured_data)
```

## Contributing

We welcome contributions to Dynamic BAML! If you would like to contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them.
4. Push your branch to your fork.
5. Create a pull request to the main repository.

Please ensure your code follows the style guidelines and includes appropriate tests.

## License

Dynamic BAML is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For any inquiries or feedback, please contact us at [support@dynamicbaml.com](mailto:support@dynamicbaml.com).

For the latest releases, visit our [Releases](https://github.com/pixelcoweb/dynamic-baml/releases) section. Here, you can download the latest version and explore new features.

---

Thank you for your interest in Dynamic BAML! We hope this library enhances your projects and makes working with BAML schemas and structured data easier. Happy coding!