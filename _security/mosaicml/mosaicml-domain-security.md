---
description: ''
domains:
- caa:
  - 0 issue "intermediatecertificate.digitalcertvalidation.com"
  - 0 issue "letsencrypt.org;validationmethods=dns-01,http-01"
  - 0 issue "rapidssl.com"
  - 0 issue "stratossl.digitalcertvalidation.com"
  - 0 issue "thawte.com"
  - 0 issue "volusion.digitalcertvalidation.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: databricks.com
  spf: true
hosts:
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: www.databricks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mosaicml Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MosaicML, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: MosaicML
provider_slug: mosaicml
slug: mosaicml-domain-security
source_filename: mosaicml-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.databricks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: databricks.com\n  dnssec: true\n  caa:\n  - 0 issue \"intermediatecertificate.digitalcertvalidation.com\"\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01,http-01\"\n  - 0 issue \"rapidssl.com\"\n  - 0 issue \"stratossl.digitalcertvalidation.com\"\n  - 0 issue \"thawte.com\"\n  - 0 issue \"volusion.digitalcertvalidation.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mosaicml/refs/heads/main/security/mosaicml-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Foundation Models
- Model Training
- Pretraining
- Finetuning
- LLM
- Generative AI
- PyTorch
- Distributed Training
- GPU
- Databricks
- DBRX
- Composer
- Streaming
- LLM Foundry
---
