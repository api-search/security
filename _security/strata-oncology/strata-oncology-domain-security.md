---
api_specs:
- filename: strata-oncology-content-api-openapi.yml
  format: yaml
  label: Strata Oncology Website Content API
  slug: strata-oncology-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/strata-oncology/refs/heads/main/openapi/strata-oncology-content-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: strataoncology.com
  spf: true
hosts:
- cert_expires: Sep 20 00:04:43 2026 GMT
  host: strataoncology.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Strata Oncology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Strata Oncology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Strata Oncology
provider_slug: strata-oncology
slug: strata-oncology-domain-security
source_filename: strata-oncology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: strataoncology.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 00:04:43 2026 GMT\n  hsts: false\ndomains:\n- domain: strataoncology.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/strata-oncology/refs/heads/main/security/strata-oncology-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Precision Medicine
- Oncology
- Genomics
- Diagnostics
- Laboratory
- Life Sciences
- Biomarkers
- Clinical Trials
---
