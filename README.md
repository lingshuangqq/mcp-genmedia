# MCP Servers for Google Cloud Genmedia APIs

This repository provides Model Context Protocol (MCP) servers that enable AI agents and applications to easily integrate and leverage Google Cloud's powerful generative media APIs (Imagen, Veo, Chirp, Lyria) and advanced audio/video compositing capabilities (AVTool).

Each server can be enabled and run separately, allowing flexibility for environments that don't require all capabilities.

## Generative Media & Compositing Capabilities

*   **[Gemini 3.0 Pro Preview](https://cloud.google.com/vertex-ai/generative-ai/docs/models/gemini/3-pro)** - for advanced reasoning and multimodal generation
*   **[Imagen 4](https://cloud.google.com/vertex-ai/generative-ai/docs/models/imagen/4)** - for image generation and editing
*   **[Veo 3.1](https://cloud.google.com/vertex-ai/generative-ai/docs/models/veo/3-1)** - for video creation
*   **[Chirp 3 HD](https://cloud.google.com/vertex-ai/generative-ai/docs/models/chirp/3-hd)** - for audio synthesis
*   **[Lyria](https://cloud.google.com/vertex-ai/generative-ai/docs/models/lyria)** - for music generation
*   **AVTool** - for audio/video compositing and manipulation

## Installation

For detailed installation instructions, including an easy-to-use installer script, please refer to the [Go Implementations README](./mcp-genmedia-go/README.md).

**Quick Start:**

1.  Navigate to the Go implementation directory:
    ```bash
    cd mcp-genmedia-go
    ```
2.  Run the installer script:
    ```bash
    ./install.sh
    ```

## Available MCP Servers

*   **`mcp-avtool-go`**: Audio/video compositing and manipulation (FFmpeg wrapper).
*   **`mcp-chirp3-go`**: Text-to-Speech synthesis using Chirp 3 HD.
*   **`mcp-gemini-go`**: Multimodal generation (text, images, audio) using Gemini 3.0 Pro Preview.
*   **`mcp-imagen-go`**: Image generation using Imagen 4.
*   **`mcp-lyria-go`**: Music generation using Lyria.
*   **`mcp-veo-go`**: Video generation using Veo 3.1.

For a detailed list of tools provided by each server, refer to the [Go Implementations README](./mcp-genmedia-go/README.md).

## Client Configurations

The MCP servers can be used with various clients and hosts. A sample MCP configuration JSON can be found at [genmedia-config.json](./sample-agents/mcp-inspector/genmedia-config.json).

This repository provides AI application samples for:

*   [Google ADK (Agent Development Kit)](./sample-agents/adk/README.md)
*   [Google Firebase Genkit](./sample-agents/genkit/README.md)
*   [Google Gemini CLI](./sample-agents/geminicli/README.md)
*   [MCP Inspector](./sample-agents/mcp-inspector/README.md)

## Development and Contribution

For those interested in extending the existing servers or creating new ones, the `mcp-genmedia-go` directory contains a more detailed `README.md` with information on the architecture and development process. Please refer to the [mcp-genmedia-go/README.md](./mcp-genmedia-go/README.md) for more information.

## License

Apache 2.0

## Disclaimer

This is not an officially supported Google product.