---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Spideroak Authentication
name_suffix: Authentication
oauth_flows: []
overview: SpiderOak declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: SpiderOak
provider_slug: spideroak
scheme_count: 4
schemes:
- description: Each Aranya device generates and holds a key bundle; the daemon generates and maintains the cryptographic keys used to encrypt and decrypt data for Aranya and Fast Channels. The device identity (AranyaDeviceId) is derived from it.
  id: device-key-bundle
  operations:
  - aranya_get_key_bundle
  - aranya_get_public_key_bundle
  - aranya_get_device_id
  - aranya_team_device_keybundle
  - aranya_team_device_public_key_bundle
  type: cryptographic-identity
- description: Joining or creating a team over the QUIC syncer requires a sync seed. A team creator generates one (aranya_create_team_quic_sync_config_generate) or supplies raw seed IKM; a joining device supplies the wrapped seed. The glossary defines PSK as "a key shared by two parties. The QUIC syncer uses PSKs instead of certificates." Seed length is fixed at ARANYA_SEED_IKM_LEN (32 bytes).
  id: quic-sync-psk-seed
  operations:
  - aranya_create_team_quic_sync_config_generate
  - aranya_create_team_quic_sync_config_raw_seed_ikm
  - aranya_add_team_quic_sync_config_wrapped_seed
  - aranya_add_team_quic_sync_config_raw_seed_ikm
  - aranya_encrypt_psk_seed_for_peer
  type: pre-shared-key
- description: 'v7.0.1 (2026-08-12) changed peer sync to use certificate-based mTLS ("use certificate-based mTLS for sync", PR #786). A certificate generation tool (aranya-certgen) was introduced in v5.0.0. See also the published mTLS specification at https://aranya-project.github.io/mtls/.'
  id: mtls-sync
  operations: []
  since: v7.0.1
  type: mutual-tls
- description: 'The client authenticates to nothing over the network to reach the daemon: it connects to a local Unix domain socket whose path the caller sets explicitly. Trust is filesystem-scoped. A failure to reach it returns ARANYA_ERROR_IPC.'
  id: daemon-uds
  operations:
  - aranya_client_config_builder_set_daemon_uds_path
  type: local-ipc
slug: spideroak-authentication
source_filename: spideroak-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://aranya-project.github.io/core-concepts/onboarding, https://aranya-project.github.io/core-concepts/access-management,\n  https://github.com/aranya-project/aranya/releases/tag/v7.0.1, capi/spideroak-aranya-client.h\ndocs: https://aranya-project.github.io/core-concepts/access-management\nprovider: SpiderOak\napi: Aranya Client API\nnote: 'Aranya has no HTTP surface and therefore no OpenAPI securitySchemes, no API keys, no bearer tokens and no\n  OAuth. Its authentication model is cryptographic and peer-to-peer: every device carries a key bundle and a device\n  identity, teams are created and joined with a QUIC sync seed, and peer sync is authenticated with certificate-based\n  mTLS as of v7.0.1. Authorization is policy-evaluated RBAC/ABAC on the Aranya graph. This artifact is written from\n  the provider''s own docs and the published C header, not derived from a spec.'\nschemes:\n- id: device-key-bundle\n  type: cryptographic-identity\n\
  \  description: Each Aranya device generates and holds a key bundle; the daemon generates and maintains the cryptographic\n    keys used to encrypt and decrypt data for Aranya and Fast Channels. The device identity (AranyaDeviceId) is\n    derived from it.\n  operations:\n  - aranya_get_key_bundle\n  - aranya_get_public_key_bundle\n  - aranya_get_device_id\n  - aranya_team_device_keybundle\n  - aranya_team_device_public_key_bundle\n- id: quic-sync-psk-seed\n  type: pre-shared-key\n  description: Joining or creating a team over the QUIC syncer requires a sync seed. A team creator generates one\n    (aranya_create_team_quic_sync_config_generate) or supplies raw seed IKM; a joining device supplies the wrapped\n    seed. The glossary defines PSK as \"a key shared by two parties. The QUIC syncer uses PSKs instead of certificates.\"\n    Seed length is fixed at ARANYA_SEED_IKM_LEN (32 bytes).\n  operations:\n  - aranya_create_team_quic_sync_config_generate\n  - aranya_create_team_quic_sync_config_raw_seed_ikm\n\
  \  - aranya_add_team_quic_sync_config_wrapped_seed\n  - aranya_add_team_quic_sync_config_raw_seed_ikm\n  - aranya_encrypt_psk_seed_for_peer\n- id: mtls-sync\n  type: mutual-tls\n  description: 'v7.0.1 (2026-08-12) changed peer sync to use certificate-based mTLS (\"use certificate-based mTLS\n    for sync\", PR #786). A certificate generation tool (aranya-certgen) was introduced in v5.0.0. See also the published\n    mTLS specification at https://aranya-project.github.io/mtls/.'\n  since: v7.0.1\n  operations: []\n- id: daemon-uds\n  type: local-ipc\n  description: 'The client authenticates to nothing over the network to reach the daemon: it connects to a local\n    Unix domain socket whose path the caller sets explicitly. Trust is filesystem-scoped. A failure to reach it\n    returns ARANYA_ERROR_IPC.'\n  operations:\n  - aranya_client_config_builder_set_daemon_uds_path\nauthorization:\n  model: policy-evaluated RBAC with rank-based authorization, plus label-based ABAC segmentation\n \
  \ description: Roles and permissions are defined in the Aranya policy language and evaluated by the policy VM. v4.0.0\n    introduced custom roles with a default set initialized by setup_default_roles(); v6.0.0 changed custom roles\n    to numerical rank-based authorization. Labels bind a data-plane channel to a set of policy rules, extending\n    graph authority into the data plane.\n  operations:\n  - aranya_setup_default_roles\n  - aranya_create_role\n  - aranya_delete_role\n  - aranya_assign_role\n  - aranya_revoke_role\n  - aranya_change_role\n  - aranya_add_perm_to_role\n  - aranya_remove_perm_from_role\n  - aranya_query_role_perms\n  - aranya_change_rank\n  - aranya_query_rank\n  - aranya_create_label\n  - aranya_delete_label\n  - aranya_assign_label\n  - aranya_revoke_label\n  docs: https://github.com/aranya-project/aranya/blob/main/crates/aranya-daemon/src/policy.md\noauth: false\napi_keys: false\nbearer_tokens: false\nmtls: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spideroak/refs/heads/main/authentication/spideroak-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Security
- Zero Trust
- Encryption
- Access Control
- Identity and Access Management
- Cryptography
- Defense
- Aerospace
- Space
- Open-Source
- Edge Computing
- Data Exchange
- Backup and Storage
---
