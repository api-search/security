---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ms.gov.pl
  spf: true
hosts:
- cert_expires: Dec 24 13:02:50 2026 GMT
  host: api-krs.ms.gov.pl
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Krajowy Rejestr Sądowy (National Court Register), Poland Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Krajowy Rejestr Sądowy (National Court Register), Poland, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Krajowy Rejestr Sądowy (National Court Register), Poland
provider_slug: api-krs-ms-gov-pl
slug: api-krs-ms-gov-pl-domain-security
source_filename: api-krs-ms-gov-pl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api-krs.ms.gov.pl\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 24 13:02:50 2026 GMT\n  hsts: null\ndomains:\n- domain: ms.gov.pl\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/api-krs-ms-gov-pl/security/api-krs-ms-gov-pl-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Government
- Business Registry
- Open Data
- Poland
- Legal Entities
- Europe
---
