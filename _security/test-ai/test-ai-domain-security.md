---
api_specs:
- filename: test-ai-opentestdata-openapi.yaml
  format: yaml
  label: OpenTestData API
  slug: opentestdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/test-ai/refs/heads/main/openapi/test-ai-opentestdata-openapi.yaml
description: ''
domains: []
hosts:
- caa:
    present: false
    records: []
  dmarc:
    present: false
    records: []
  dnssec:
    enabled: false
    evidence: 'No DS record; registry whois reports "DNSSEC: unsigned".'
  host: test.ai
  hsts:
    evidence: No Strict-Transport-Security header on the port-80 response, whose Server header is namecheap-nginx.
    present: false
  http:
    behaviour: Blanket catch-all 302 to https://icebergqa.com/?utm_source=testai&utm_medium=redir for every path probed, including /robots.txt. No path serves origin content.
    port_80: open
  ip: 192.64.119.35
  mx:
    note: No MX records — the domain cannot receive mail.
    present: false
    records: []
  registrar:
    expires: '2027-01-19'
    name: NameCheap, Inc.
    nameservers:
    - dns1.registrar-servers.com
    - dns2.registrar-servers.com
    status:
    - clientTransferProhibited
    updated: '2026-08-12'
  spf:
    present: false
    records: []
  tls:
    available: false
    certificate: null
    evidence: curl and a raw TCP connect to 192.64.119.35:443 both time out after 10s; port 80 accepts immediately from the same client, so this is a filtered/absent listener rather than a network fault at our end.
    port_443: filtered
- evidence: NXDOMAIN — no A, AAAA or CNAME. No TLS, DNS or HTTP posture can be measured.
  host: api.opentestdata.org
  resolves: false
kind: domain-security
layout: security
method: probed
name: Test Ai Domain Security
name_suffix: Domain Security
overview: Domain security posture for test.ai, probed live across 2 host(s) and 0 registrable domain(s).
provider_name: test.ai
provider_slug: test-ai
slug: test-ai-domain-security
source_filename: test-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: 'probed 2026-08-30: TCP/TLS to test.ai:443, DNS (A/MX/TXT/CAA/DS), whois.nic.ai'\nnote: >-\n  0-working/probe-domain-security.py returned `unreachable` and wrote nothing, so this file was\n  written by hand from the raw probes. The unreachability IS the finding: test.ai has no HTTPS\n  service at all. Every negative below is a real observation, not an unattempted check.\nhosts:\n- host: test.ai\n  ip: 192.64.119.35\n  tls:\n    available: false\n    port_443: filtered\n    evidence: >-\n      curl and a raw TCP connect to 192.64.119.35:443 both time out after 10s; port 80 accepts\n      immediately from the same client, so this is a filtered/absent listener rather than a\n      network fault at our end.\n    certificate: null\n  hsts:\n    present: false\n    evidence: >-\n      No Strict-Transport-Security header on the port-80 response, whose Server header is\n      namecheap-nginx.\n  http:\n    port_80: open\n    behaviour:\
  \ >-\n      Blanket catch-all 302 to https://icebergqa.com/?utm_source=testai&utm_medium=redir for every\n      path probed, including /robots.txt. No path serves origin content.\n  dnssec:\n    enabled: false\n    evidence: 'No DS record; registry whois reports \"DNSSEC: unsigned\".'\n  caa:\n    present: false\n    records: []\n  spf:\n    present: false\n    records: []\n  dmarc:\n    present: false\n    records: []\n  mx:\n    present: false\n    records: []\n    note: No MX records — the domain cannot receive mail.\n  registrar:\n    name: NameCheap, Inc.\n    nameservers:\n    - dns1.registrar-servers.com\n    - dns2.registrar-servers.com\n    updated: '2026-08-12'\n    expires: '2027-01-19'\n    status:\n    - clientTransferProhibited\n- host: api.opentestdata.org\n  resolves: false\n  evidence: NXDOMAIN — no A, AAAA or CNAME. No TLS, DNS or HTTP posture can be measured.\nsubdomains_probed:\n  result: none resolve\n  hosts:\n  - api.test.ai\n  - docs.test.ai\n  - app.test.ai\n \
  \ - developer.test.ai\n  - dev.test.ai\n  - status.test.ai\n  - blog.test.ai\n  - mcp.test.ai\n  - sdk.test.ai\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/test-ai/refs/heads/main/security/test-ai-domain-security.yml
summary_line: HSTS
tags:
- Company
- Testing
- Test Automation
- Quality Assurance
- Artificial Intelligence
- Machine-Learning
- Computer-Vision
- Selenium
- Appium
- Developer Tools
- gRPC
- Defunct
---
