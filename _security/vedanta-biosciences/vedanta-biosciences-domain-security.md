---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: vedantabio.com
  spf: true
hosts:
- cert_expires: Sep 20 01:44:10 2026 GMT
  host: www.vedantabio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vedanta Biosciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vedanta Biosciences, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Vedanta Biosciences
provider_slug: vedanta-biosciences
slug: vedanta-biosciences-domain-security
source_filename: vedanta-biosciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vedantabio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 01:44:10 2026 GMT\n  hsts: false\ndomains:\n- domain: vedantabio.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vedanta-biosciences/refs/heads/main/security/vedanta-biosciences-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Biotechnology
- Life Sciences
- Pharmaceuticals
- Microbiome
- Live Biotherapeutic Products
- Immunology
- Gastroenterology
- Infectious Disease
- Clinical Research
- Drug Development
- Health Care
- United States
---
