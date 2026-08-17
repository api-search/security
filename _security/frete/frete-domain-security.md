---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: frete.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fretebras.com.br
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:_spf.rdstation.com.br include:spf1.neoassist.com include:9020753.spf04.hubspotemail.net include:one.zoho.com include:mail.zendesk.com include:_spf.qp-mail.com -all
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cargox.com.br
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:sendgrid.net include:_spf.salesforce.com include:_spf.qp-mail.mx include:one.zoho.com -all
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fretepago.com.br
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:amazonses.com -all
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rotasbrasil.com.br
  spf: true
  spf_record: v=spf1 include:websitewelcome.com -all
hosts:
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: www.frete.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: www.fretebras.com.br
  hsts: null
  https: true
  note: Akamai edge answered HTTP 403 (Access Denied) to the probe; headers beyond the challenge response were not observable.
- host: cargox.com.br
  hsts: max-age=2628000
  https: true
  note: HTTP 200; HSTS max-age 2628000 (~30 days), no includeSubDomains, no preload.
- host: api.fretepago.com.br
  hsts: null
  https: true
  note: Akamai edge answered HTTP 403 (Access Denied) to the probe; no public API surface observable.
kind: domain-security
layout: security
method: probed
name: Frete Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Frete.com, probed live across 4 host(s) and 5 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Frete.com
provider_slug: frete
slug: frete-domain-security
source_filename: frete-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts plus the Frete.com brand domains (fretebras.com.br, cargox.com.br, fretepago.com.br, rotasbrasil.com.br)\nhosts:\n- host: www.frete.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: null\n- host: www.fretebras.com.br\n  https: true\n  hsts: null\n  note: 'Akamai edge answered HTTP 403 (Access Denied) to the probe; headers beyond the challenge response were not observable.'\n- host: cargox.com.br\n  https: true\n  hsts: 'max-age=2628000'\n  note: 'HTTP 200; HSTS max-age 2628000 (~30 days), no includeSubDomains, no preload.'\n- host: api.fretepago.com.br\n  https: true\n  hsts: null\n  note: 'Akamai edge answered HTTP 403 (Access Denied) to the probe; no public API surface observable.'\ndomains:\n- domain: frete.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: fretebras.com.br\n  dnssec: false\n  caa:\
  \ []\n  spf: true\n  spf_record: 'v=spf1 include:_spf.google.com include:_spf.rdstation.com.br include:spf1.neoassist.com include:9020753.spf04.hubspotemail.net include:one.zoho.com include:mail.zendesk.com include:_spf.qp-mail.com -all'\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: cargox.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 include:_spf.google.com include:sendgrid.net include:_spf.salesforce.com include:_spf.qp-mail.mx include:one.zoho.com -all'\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: fretepago.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 include:_spf.google.com include:amazonses.com -all'\n  dmarc: true\n  dmarc_policy: reject\n- domain: rotasbrasil.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 include:websitewelcome.com -all'\n  dmarc: true\n  dmarc_policy: none\nfindings:\n- 'Only the primary frete.com zone is DNSSEC-signed; none of the four Brazilian brand domains are.'\n- 'No\
  \ CAA records are published on any of the five domains.'\n- 'SPF and DMARC are published everywhere; DMARC enforcement varies from p=reject (frete.com, fretepago.com.br) to p=none (rotasbrasil.com.br, the most recently acquired brand).'\n- 'HSTS was observable only on cargox.com.br (max-age ~30 days, no includeSubDomains, no preload). The Akamai-fronted hosts returned a 403 challenge to the probe.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frete/refs/heads/main/security/frete-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Logistics
- Freight
- Transportation
- Trucking
- Marketplace
- Supply Chain
- Fintech
- Brazil
- Latin America
- Machine Learning
---
