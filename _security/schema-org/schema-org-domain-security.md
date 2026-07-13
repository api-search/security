---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: schema.org
  spf: true
hosts:
- cert_expires: Sep 14 08:37:49 2026 GMT
  host: schema.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:37:49 2026 GMT
  host: validator.schema.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Schema Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Schema.org, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Schema.org
provider_slug: schema-org
slug: schema-org-domain-security
source_filename: schema-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: schema.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:37:49 2026 GMT\n  hsts: false\n- host: validator.schema.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:37:49 2026 GMT\n  hsts: false\ndomains:\n- domain: schema.org\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/security/schema-org-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Schema.org
- Structured Data
- Linked Data
- JSON-LD
- Vocabulary
- SEO
- Web Standards
- RDF
- Ontology
---
