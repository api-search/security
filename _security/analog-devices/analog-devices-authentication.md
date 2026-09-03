---
api_key_in: []
auth_types: []
description: Most Analog Devices developer software carries no authentication at all — libiio, pyadi-iio and no-OS are local libraries that talk to silicon over USB, SPI, I2C or a network daemon, and the iiod daemon has no built-in authentication (the published guidance is to wrap it in stunnel). The one real authentication surface ADI documents is myAnalog, which gates the CodeFusion Studio Package Manager's restricted package remotes. It supports an interactive browser login and, for CI/CD, long-lived API keys managed through cfsutil.
kind: authentication
layout: security
method: searched
name: Analog Devices Authentication
name_suffix: Authentication
oauth_flows: []
overview: Analog Devices declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Analog Devices
provider_slug: analog-devices
scheme_count: 2
schemes:
- command_palette:
  - (CFS) myAnalog Login
  - (CFS) myAnalog Status
  commands:
  - cfsutil myanalog login [--verbose]
  - cfsutil myanalog status [--verbose]
  - cfsutil myanalog logout
  description: cfsutil or the VS Code Command Palette opens an external browser at the myAnalog sign-in page; on success the session is written back to the client and the managed package remotes are configured automatically.
  docs: https://developer.analog.com/docs/codefusion-studio/latest/user-guide/installation/package-manager/auth/
  id: myanalog-interactive
  identity_providers:
  - Email and password (myAnalog account, register at analog.com/myAnalog)
  - Google Account
  - LinkedIn Account
  - Analog Devices Account (employees and contractors on managed devices)
  name: myAnalog interactive login
  note: ADI does not publish an OAuth authorization-server metadata document, token endpoint, or scope reference for this flow — /.well-known/ openid-configuration and /oauth-authorization-server were probed on developer.analog.com (SPA shell), api.analog.com (403) and www.analog.com (no response). The flow is documented in prose only, so no scopes/ artifact is emitted.
  type: browser-redirect
- commands:
  - cfsutil myanalog apikey create [--description <description>]
  - cfsutil myanalog apikey list
  - cfsutil myanalog apikey delete <key-id>
  covered_commands:
  - catalog update
  - ai build
  - docker pull
  - package manager commands
  description: Long-lived API key for non-interactive use in automated workflows and CI/CD pipelines. The key value is displayed exactly once at creation and cannot be retrieved afterwards.
  docs: https://developer.analog.com/docs/codefusion-studio/latest/user-guide/cfsutil/apikey-auth/
  id: cfs-api-key
  in: environment
  key_id_format: apikey_<id>
  lifecycle:
    creation_requires: an active myAnalog session (cfsutil myanalog login)
    expiration: Keys carry an expiration date shown by `apikey list`; the documentation does not state the default lifetime.
    listing_shows: key id, masked value, expiration date
    revocation: cfsutil myanalog apikey delete <key-id>
  name: CFS_API_KEY
  supported_by: cfsutil only — the VS Code extension does not accept API keys
  type: apiKey
  usage: CFS_API_KEY=<your-api-key> cfsutil catalog update
slug: analog-devices-authentication
source_filename: analog-devices-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: >-\n  https://developer.analog.com/docs/codefusion-studio/latest/user-guide/cfsutil/apikey-auth/,\n  .../user-guide/cfsutil/myanalog-auth/ and\n  .../user-guide/installation/package-manager/auth/\nprovider: Analog Devices\nproviderId: analog-devices\ndescription: >-\n  Most Analog Devices developer software carries no authentication at all —\n  libiio, pyadi-iio and no-OS are local libraries that talk to silicon over\n  USB, SPI, I2C or a network daemon, and the iiod daemon has no built-in\n  authentication (the published guidance is to wrap it in stunnel). The one\n  real authentication surface ADI documents is myAnalog, which gates the\n  CodeFusion Studio Package Manager's restricted package remotes. It supports\n  an interactive browser login and, for CI/CD, long-lived API keys managed\n  through cfsutil.\nschemes:\n  - id: myanalog-interactive\n    type: browser-redirect\n    name: myAnalog interactive login\n    description:\
  \ >-\n      cfsutil or the VS Code Command Palette opens an external browser at the\n      myAnalog sign-in page; on success the session is written back to the\n      client and the managed package remotes are configured automatically.\n    identity_providers:\n      - Email and password (myAnalog account, register at analog.com/myAnalog)\n      - Google Account\n      - LinkedIn Account\n      - Analog Devices Account (employees and contractors on managed devices)\n    commands:\n      - cfsutil myanalog login [--verbose]\n      - cfsutil myanalog status [--verbose]\n      - cfsutil myanalog logout\n    command_palette:\n      - (CFS) myAnalog Login\n      - (CFS) myAnalog Status\n    docs: https://developer.analog.com/docs/codefusion-studio/latest/user-guide/installation/package-manager/auth/\n    note: >-\n      ADI does not publish an OAuth authorization-server metadata document,\n      token endpoint, or scope reference for this flow — /.well-known/\n      openid-configuration and\
  \ /oauth-authorization-server were probed on\n      developer.analog.com (SPA shell), api.analog.com (403) and\n      www.analog.com (no response). The flow is documented in prose only, so\n      no scopes/ artifact is emitted.\n  - id: cfs-api-key\n    type: apiKey\n    in: environment\n    name: CFS_API_KEY\n    description: >-\n      Long-lived API key for non-interactive use in automated workflows and\n      CI/CD pipelines. The key value is displayed exactly once at creation and\n      cannot be retrieved afterwards.\n    supported_by: cfsutil only — the VS Code extension does not accept API keys\n    commands:\n      - cfsutil myanalog apikey create [--description <description>]\n      - cfsutil myanalog apikey list\n      - cfsutil myanalog apikey delete <key-id>\n    key_id_format: apikey_<id>\n    usage: 'CFS_API_KEY=<your-api-key> cfsutil catalog update'\n    covered_commands:\n      - catalog update\n      - ai build\n      - docker pull\n      - package manager commands\n \
  \   lifecycle:\n      creation_requires: an active myAnalog session (cfsutil myanalog login)\n      listing_shows: key id, masked value, expiration date\n      revocation: cfsutil myanalog apikey delete <key-id>\n      expiration: >-\n        Keys carry an expiration date shown by `apikey list`; the documentation\n        does not state the default lifetime.\n    docs: https://developer.analog.com/docs/codefusion-studio/latest/user-guide/cfsutil/apikey-auth/\nunauthenticated_surfaces:\n  - name: libiio local context\n    note: >-\n      Local, USB and XML contexts require no credentials; access is governed by\n      OS device permissions.\n  - name: iiod network daemon\n    note: >-\n      The libiio server daemon exposes an IIO context over the network with no\n      built-in authentication. The published mitigation is to encrypt and front\n      it with stunnel — see \"Encrypting Connections to iiod with stunnel\" in the\n      libiio documentation.\n  - name: pyadi-iio\n    note: Wraps\
  \ libiio contexts; inherits the same no-credential model.\ngated_surfaces:\n  - host: api.analog.com\n    note: >-\n      A real ADI API host (Akamai) that returns 403 for every anonymous request,\n      including /.well-known/*. Its authentication model is not published\n      anywhere this pass could read; the corporate site page that describes\n      ADI's API suites (www.analog.com/en/support/api-suites.html) could not be\n      fetched — the edge reset the connection.\nmaintainers:\n  - FN: API Evangelist\n    email: info@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/analog-devices/refs/heads/main/authentication/analog-devices-authentication.yml
summary_line: 2 schemes
tags:
- Embedded Systems
- Hardware
- IoT
- Semiconductors
- Signal Processing
- Fortune 1000
---
