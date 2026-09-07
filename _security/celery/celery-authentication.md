---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Celery Authentication
name_suffix: Authentication
oauth_flows: []
overview: Celery declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Celery
provider_slug: celery
scheme_count: 3
schemes:
- docs: https://docs.celeryq.dev/en/stable/userguide/security.html
  example_shape: amqp://<user>:<password>@<host>:5672/<vhost> or redis://:<password>@<host>:6379/0
  id: broker-credentials
  location: connection URL
  note: The documentation is explicit that the broker must be firewalled and that fine-grained broker access control (the RabbitMQ example is given) should be enabled — the broker is the trust boundary, and by default "workers trust that the data they get from the broker hasn't been tampered with".
  tls: broker_use_ssl — end-to-end SSL encryption and authentication where the broker backend supports it
  type: transport-credentials
- id: result-backend-credentials
  location: result_backend connection URL
  note: Same shape as the broker URL; credentials are carried in the DSN.
  type: transport-credentials
- activation: app.setup_security() — also disables all insecure serializers on the worker
  docs: https://docs.celeryq.dev/en/stable/userguide/security.html
  id: message-signing
  library: cryptography (PyPI)
  mechanism: Clients sign each message with a private key; workers verify it against a public certificate. Certificates may be CA-signed or self-signed. The auth serializer signs but does NOT encrypt — the docs state confidentiality must be arranged separately.
  serializer: auth
  settings:
  - name: task_serializer
    value: auth
  - name: event_serializer
    note: Additionally signs the event protocol.
    value: auth
  - name: accept_content
    note: Forces workers to accept only signed messages.
    value: '[''auth'']'
  - description: Path to the private key on the filesystem (absolute paths recommended).
    name: security_key
  - description: Password for an encrypted private key.
    name: security_key_password
  - description: Path to this node's certificate.
    name: security_certificate
  - description: Glob of trusted certificates, e.g. /etc/ssl/certs/*.pem.
    name: security_cert_store
  - description: Signing digest algorithm, e.g. sha256.
    name: security_digest
  type: public-key-message-signing
slug: celery-authentication
source_filename: celery-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: >-\n  https://docs.celeryq.dev/en/stable/userguide/security.html,\n  https://docs.celeryq.dev/en/stable/userguide/configuration.html\nsummary: >-\n  Celery has no HTTP surface and therefore no API keys, bearer tokens, OAuth flows or\n  securitySchemes. Authentication in Celery is two separate things: credentials on the BROKER and\n  RESULT BACKEND connection URLs, and optional cryptographic signing of the task and event messages\n  themselves so a worker will only execute messages it can verify.\nschemes:\n  - id: broker-credentials\n    type: transport-credentials\n    location: connection URL\n    example_shape: 'amqp://<user>:<password>@<host>:5672/<vhost> or redis://:<password>@<host>:6379/0'\n    tls: broker_use_ssl — end-to-end SSL encryption and authentication where the broker backend supports it\n    docs: https://docs.celeryq.dev/en/stable/userguide/security.html\n    note: >-\n      The documentation is explicit that\
  \ the broker must be firewalled and that fine-grained broker\n      access control (the RabbitMQ example is given) should be enabled — the broker is the trust\n      boundary, and by default \"workers trust that the data they get from the broker hasn't been\n      tampered with\".\n  - id: result-backend-credentials\n    type: transport-credentials\n    location: result_backend connection URL\n    note: Same shape as the broker URL; credentials are carried in the DSN.\n  - id: message-signing\n    type: public-key-message-signing\n    serializer: auth\n    library: cryptography (PyPI)\n    mechanism: >-\n      Clients sign each message with a private key; workers verify it against a public certificate.\n      Certificates may be CA-signed or self-signed. The auth serializer signs but does NOT encrypt —\n      the docs state confidentiality must be arranged separately.\n    settings:\n      - name: task_serializer\n        value: auth\n      - name: event_serializer\n        value: auth\n\
  \        note: Additionally signs the event protocol.\n      - name: accept_content\n        value: \"['auth']\"\n        note: Forces workers to accept only signed messages.\n      - name: security_key\n        description: Path to the private key on the filesystem (absolute paths recommended).\n      - name: security_key_password\n        description: Password for an encrypted private key.\n      - name: security_certificate\n        description: Path to this node's certificate.\n      - name: security_cert_store\n        description: Glob of trusted certificates, e.g. /etc/ssl/certs/*.pem.\n      - name: security_digest\n        description: Signing digest algorithm, e.g. sha256.\n    activation: app.setup_security() — also disables all insecure serializers on the worker\n    docs: https://docs.celeryq.dev/en/stable/userguide/security.html\ncontent_type_allowlist:\n  setting: accept_content\n  default: \"['json']\"\n  since: 3.0.18\n  note: >-\n    The primary hardening control. pickle\
  \ is documented as inherently insecure and to be avoided\n    whenever clients are untrusted or unauthenticated; JSON has been the default serializer since 4.0.\noauth2: false\nopenid_connect: false\napi_keys: false\nmutual_tls: partial — broker_use_ssl can carry client certificates where the transport supports it\nscopes_artifact: na — no OAuth surface, so scopes/ is deliberately absent\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/celery/refs/heads/main/authentication/celery-authentication.yml
summary_line: 3 schemes
tags:
- Asynchronous
- Distributed Systems
- Message Queue
- Open-Source
- Python
- Task Queue
---
