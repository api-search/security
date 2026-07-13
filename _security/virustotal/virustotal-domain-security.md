---
api_specs:
- filename: virustotal-access-control-openapi.yml
  format: yaml
  label: VirusTotal API v3 - Access Control
  slug: virustotal-api-v3-access-control
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virustotal/refs/heads/main/openapi/virustotal-access-control-openapi.yml
- filename: virustotal-ioc-feeds-openapi.yml
  format: yaml
  label: VirusTotal API v3 - IoC Feeds
  slug: virustotal-api-v3-ioc-feeds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virustotal/refs/heads/main/openapi/virustotal-ioc-feeds-openapi.yml
- filename: virustotal-ioc-investigation-openapi.yml
  format: yaml
  label: VirusTotal API v3 - IoC Investigation
  slug: virustotal-api-v3-ioc-investigation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virustotal/refs/heads/main/openapi/virustotal-ioc-investigation-openapi.yml
- filename: virustotal-private-scanning-openapi.yml
  format: yaml
  label: VirusTotal API v3 - Private Scanning
  slug: virustotal-api-v3-private-scanning
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virustotal/refs/heads/main/openapi/virustotal-private-scanning-openapi.yml
- filename: virustotal-threat-graphs-openapi.yml
  format: yaml
  label: VirusTotal API v3 - Threat Graphs
  slug: virustotal-api-v3-threat-graphs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virustotal/refs/heads/main/openapi/virustotal-threat-graphs-openapi.yml
- filename: virustotal-threat-landscape-openapi.yml
  format: yaml
  label: VirusTotal API v3 - Threat Landscape & Vulnerability Intelligence
  slug: virustotal-api-v3-threat-landscape-vulnerability-intelligence
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virustotal/refs/heads/main/openapi/virustotal-threat-landscape-openapi.yml
- filename: virustotal-yara-hunting-openapi.yml
  format: yaml
  label: VirusTotal API v3 - YARA Hunting (Livehunt, Retrohunt, IoC Stream)
  slug: virustotal-api-v3-yara-hunting-livehunt-retrohunt-ioc-stream
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virustotal/refs/heads/main/openapi/virustotal-yara-hunting-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: virustotal.com
  spf: true
hosts:
- cert_expires: Sep 22 03:26:46 2026 GMT
  host: www.virustotal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 13:01:52 2026 GMT
  host: docs.virustotal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 05:15:17 2026 GMT
  host: gtidocs.virustotal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Virustotal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VirusTotal, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: VirusTotal
provider_slug: virustotal
slug: virustotal-domain-security
source_filename: virustotal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.virustotal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 03:26:46 2026 GMT\n  hsts: null\n- host: docs.virustotal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 13:01:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: gtidocs.virustotal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 05:15:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: virustotal.com\n  dnssec: true\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virustotal/refs/heads/main/security/virustotal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Anti-Malware
- Threat Intelligence
- Security
- File Analysis
- URL Analysis
- YARA
- IoC
- Sandbox
- MITRE ATT&CK
- Google Cloud
---
