---
api_specs:
- filename: canonical-snapd-rest-api-openapi.yml
  format: yaml
  label: snapd REST API
  slug: snapd-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-snapd-rest-api-openapi.yml
- filename: canonical-landscape-debarchive-api-openapi.yml
  format: yaml
  label: Landscape API
  slug: landscape-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-landscape-debarchive-api-openapi.yml
- filename: canonical-assertions-api-openapi.yml
  format: yaml
  label: Canonical Assertions API
  slug: canonical-assertions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-assertions-api-openapi.yml
- filename: canonical-search-api-openapi.yml
  format: yaml
  label: Canonical Search API
  slug: canonical-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-search-api-openapi.yml
- filename: canonical-snaps-api-openapi.yml
  format: yaml
  label: Canonical Snaps API
  slug: canonical-snaps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-snaps-api-openapi.yml
- filename: canonical-lxd-rest-api-openapi.yml
  format: yaml
  label: LXD REST API
  slug: lxd-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-lxd-rest-api-openapi.yml
- filename: canonical-ubuntu-security-api-openapi.json
  format: json
  label: Ubuntu Security API
  slug: ubuntu-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-ubuntu-security-api-openapi.json
- filename: canonical-pebble-api-openapi.yml
  format: yaml
  label: Pebble API
  slug: pebble-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-pebble-api-openapi.yml
- filename: canonical-testflinger-api-openapi.json
  format: json
  label: Testflinger API
  slug: testflinger-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-testflinger-api-openapi.json
- filename: canonical-hardware-api-openapi.json
  format: json
  label: Ubuntu Hardware API (hwapi)
  slug: hardware-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-hardware-api-openapi.json
- filename: canonical-identity-platform-api-openapi.yml
  format: yaml
  label: Canonical Identity Platform API
  slug: identity-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-identity-platform-api-openapi.yml
- filename: canonical-test-observer-api-openapi.json
  format: json
  label: Test Observer API
  slug: test-observer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-test-observer-api-openapi.json
- filename: canonical-anbox-cloud-ams-api-openapi.json
  format: json
  label: Anbox Cloud AMS API
  slug: anbox-cloud-ams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-anbox-cloud-ams-api-openapi.json
- filename: canonical-anbox-stream-gateway-api-openapi.json
  format: json
  label: Anbox Stream Gateway API
  slug: anbox-stream-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-anbox-stream-gateway-api-openapi.json
- filename: canonical-cos-registration-server-api-openapi.yml
  format: yaml
  label: COS Registration Server API
  slug: cos-registration-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-cos-registration-server-api-openapi.yml
- filename: canonical-microceph-api-openapi.yml
  format: yaml
  label: MicroCeph REST API
  slug: microceph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/openapi/canonical-microceph-api-openapi.yml
certification_count: 0
certifications: []
description: 'Canonical does not operate a branded "trust center" portal (trust.canonical.com and canonical.com/trust both 404 on 2026-09-05). What it publishes instead is a security and compliance hub under ubuntu.com/security, and the distinction below is deliberate and load-bearing: some of these are CERTIFICATIONS Canonical holds for its own product, and the rest are compliance regimes Canonical sells tooling to help a CUSTOMER achieve. Conflating the two would credit Canonical with attestations it does not claim.'
kind: trust-center
layout: security
name: Canonical Trust Center
name_suffix: Trust Center
overview: Canonical maintains a public trust center covering its security and compliance posture.
provider_name: Canonical
provider_slug: canonical
slug: canonical-trust-center
source_filename: canonical-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: https://ubuntu.com/security/certifications, https://ubuntu.com/security/fips, https://ubuntu.com/security/cc,\n  https://ubuntu.com/security/esm, https://ubuntu.com/security\nprovider: Canonical\nproviderId: canonical\ndescription: 'Canonical does not operate a branded \"trust center\" portal (trust.canonical.com and canonical.com/trust\n  both 404 on 2026-09-05). What it publishes instead is a security and compliance hub under ubuntu.com/security,\n  and the distinction below is deliberate and load-bearing: some of these are CERTIFICATIONS Canonical\n  holds for its own product, and the rest are compliance regimes Canonical sells tooling to help a CUSTOMER\n  achieve. Conflating the two would credit Canonical with attestations it does not claim.'\nportal:\n  url: https://ubuntu.com/security/certifications\n  http_status: 200\n  probed: '2026-09-05'\n  branded_trust_center: false\n  probed_absent:\n  - url: https://canonical.com/trust\n\
  \    http_status: 404\n  - url: https://ubuntu.com/security/trust-center\n    http_status: 404\ncertifications_held:\n- name: FIPS 140-2\n  subject: Ubuntu cryptographic modules\n  status: certified\n  evidence: https://ubuntu.com/security/fips\n  quote: '\"FIPS 140-2 & 140-3 certified modules are available for Ubuntu.\"'\n- name: FIPS 140-3\n  subject: Ubuntu 22.04 LTS cryptographic modules\n  status: certified\n  evidence: https://ubuntu.com/security/fips\n  quote: '\"FIPS 140-3 is now available for Ubuntu 22.04 LTS.\"'\n- name: Common Criteria\n  subject: Ubuntu 18.04 LTS and Ubuntu 16.04 LTS\n  status: certified\n  evidence: https://ubuntu.com/security/cc\n  level: EAL2\n  scheme: ISO/IEC 15408; certified through CSEC (the Swedish Certification Body for IT Security), evaluated\n    by atsec Information Security\n  quote: '\"Ubuntu 18.04 LTS and 16.04 LTS have both been evaluated to assurance level EAL2 through CSEC\n    — The Swedish Certification Body for IT Security.\"'\n  note:\
  \ Both certified releases are now out of standard support; no EAL evaluation is published for 20.04,\n    22.04 or 24.04.\ncompliance_enablement:\n  note: Canonical publishes tooling and hardening automation for these regimes. These are NOT Canonical\n    certifications; the page's own wording is that Canonical \"helps you comply\" or \"supports your path\n    towards\" them.\n  regimes:\n  - name: DISA-STIG\n    tooling: Ubuntu Security Guide (USG)\n  - name: CIS Benchmarks\n    tooling: Ubuntu Security Guide (USG)\n  - name: FedRAMP\n    note: '\"Find security tools to help you achieve FedRAMP Authority To Operate.\"'\n  - name: PCI-DSS\n  - name: HIPAA\n    note: '\"Canonical supports your path towards HIPAA compliance.\"'\n  - name: NIST 800-53\n  - name: CMMC\n  - name: EU Cyber Resilience Act (CRA)\n    evidence: https://canonical.com/solutions/open-source-security/cyber-resilience-act\n  - name: EU NIS2\n  - name: UK Cyber Essentials\nnot_found:\n- name: SOC 2\n  note: No SOC 2\
  \ report or attestation is advertised on ubuntu.com/security; ubuntu.com/security/soc-2\n    returned 404 on 2026-09-05.\n- name: ISO 27001\n  note: Not named on the certifications page; ubuntu.com/security/iso-27001 returned 404 on 2026-09-05.\n    Absence of a published page is not proof Canonical lacks the certificate — only that it is not published\n    where a buyer or an agent would look.\nsubprocessors_or_dpa:\n  privacy_policy: https://ubuntu.com/legal/data-privacy\n  terms: https://ubuntu.com/legal/terms\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canonical/refs/heads/main/security/canonical-trust-center.yml
summary_line: trust center published
tags:
- Cloud
- Linux
- Open-Source
- Ubuntu
- Containers
- Bare Metal
- Charms
- Identity
trust_url: ''
---
