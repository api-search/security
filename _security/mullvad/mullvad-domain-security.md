---
api_specs:
- filename: mullvad-openapi-generated.yml
  format: yaml
  label: Mullvad VPN API
  slug: mullvad-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mullvad/openapi/_ae-authored/mullvad-openapi-generated.yml
description: ''
domains:
- caa:
  - 128 issue "letsencrypt.org"
  - 128 iodef "mailto:support@mullvadvpn.net"
  - 128 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: mullvad.net
  spf: true
hosts:
- cert_expires: Jan  7 07:58:11 2027 GMT
  host: mullvad.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mullvad Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mullvad VPN, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Mullvad VPN
provider_slug: mullvad
slug: mullvad-domain-security
source_filename: mullvad-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mullvad.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 07:58:11 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mullvad.net\n  dnssec: true\n  caa:\n  - 128 issue \"letsencrypt.org\"\n  - 128 iodef \"mailto:support@mullvadvpn.net\"\n  - 128 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/mullvad/security/mullvad-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- VPN
- Privacy
- OpenSource
- Security
---
