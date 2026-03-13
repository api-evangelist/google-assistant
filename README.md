# Google Assistant API

The Google Assistant API enables developers to embed the Google Assistant into devices and applications. It provides conversational interfaces through gRPC and REST endpoints for sending text or audio queries and receiving responses. The API supports device model and instance registration, custom Actions with intents and scenes, and the Actions SDK for building conversational experiences that extend the Assistant's capabilities.

## Artifacts

- **APIs.yml** - Machine-readable API metadata following the APIs.json specification.
- **OpenAPI** (`openapi/openapi.yml`) - OpenAPI 3.1.0 specification describing the Assistant API endpoints for device management and conversational interactions.
- **JSON Schema** (`json-schema/google-assistant.json`) - JSON Schema (draft 2020-12) defining device model, device instance, and conversation objects.
- **JSON-LD** (`json-ld/google-assistant.jsonld`) - JSON-LD context mapping Assistant API terms to schema.org and API-specific vocabularies.

## Key Endpoints

| Method | Path | Description |
|--------|------|-------------|
| GET | `/v1alpha2/projects/{projectId}/deviceModels` | List device models |
| POST | `/v1alpha2/projects/{projectId}/deviceModels` | Create a device model |
| GET | `/v1alpha2/projects/{projectId}/deviceModels/{id}` | Get a device model |
| DELETE | `/v1alpha2/projects/{projectId}/deviceModels/{id}` | Delete a device model |
| GET | `/v1alpha2/projects/{projectId}/devices` | List device instances |
| POST | `/v1alpha2/projects/{projectId}/devices` | Register a device instance |

## Resources

- [Google Assistant SDK Overview](https://developers.google.com/assistant/sdk/overview)
- [Actions on Google](https://developers.google.com/assistant/actions)
- [Actions API Reference](https://developers.google.com/assistant/actions/api)

## Maintainer

Kin Lane - kin@apievangelist.com
