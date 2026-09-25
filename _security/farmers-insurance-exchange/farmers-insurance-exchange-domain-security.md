---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: farmers.com
  spf: true
  spf_record: v=spf1 include:%{ir}.%{v}.%{d}.spf.has.pphosted.com -all
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: farmersinsurance.com
  spf: true
  spf_record: v=spf1 include:%{ir}.%{v}.%{d}.spf.has.pphosted.com ~all
hosts:
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: www.farmers.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: developer.farmers.com
  hsts: null
  https: true
  note: HEAD timed out behind Akamai Bot Manager; HSTS not observed
  tls_version: TLSv1.3
- cert_expires: Dec  1 14:45:03 2026 GMT
  host: newsroom.farmers.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 21 23:59:59 2027 GMT
  host: epartner.farmersinsurance.com
  hsts: null
  https: true
  note: HEAD timed out behind the edge; redirects 303 to farmersinsurance.okta.com SAML SSO
  tls_version: TLSv1.3
- host: www.farmersinsurance.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.farmersinsurance.com'' (served cert CN=a248.e.akamai.net)'
hosts_probed: 5
kind: domain-security
layout: security
method: probed
name: Farmers Insurance Exchange Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Farmers Insurance Exchange, probed live across 5 host(s) and 2 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Farmers Insurance Exchange
provider_slug: farmers-insurance-exchange
slug: farmers-insurance-exchange-domain-security
source_filename: farmers-insurance-exchange-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: >-\n  live DNS/TLS/HTTP probes of every Farmers host this record knows — the website host from\n  apis.yml, the developer portal at developer.farmers.com, the newsroom, the ePartner SSO\n  host, and the legacy www.farmersinsurance.com host the previous revision of apis.yml\n  carried as Website.\nnote: >-\n  www.farmersinsurance.com and the farmersinsurance.com apex both terminate TLS on an Akamai\n  edge certificate (CN a248.e.akamai.net) that carries no SAN for either name, so every HTTPS\n  client rejects them. That is why the Website pointer was moved to https://www.farmers.com/,\n  which serves a valid certificate. The farmersinsurance.com domain is not dead — the\n  epartner. and jobs. subdomains under it serve valid certificates — only its apex and www\n  hosts are misconfigured. No host in the estate returns a Strict-Transport-Security header\n  on an anonymous HEAD except newsroom.farmers.com; the Akamai-fronted hosts\
  \ answer bot\n  mitigation instead of a header, so hsts is recorded null (not observed) rather than false.\nhosts:\n- host: www.farmers.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: null\n- host: developer.farmers.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: null\n  note: HEAD timed out behind Akamai Bot Manager; HSTS not observed\n- host: newsroom.farmers.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 14:45:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: epartner.farmersinsurance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 21 23:59:59 2027 GMT\n  hsts: null\n  note: HEAD timed out behind the edge; redirects 303 to farmersinsurance.okta.com SAML SSO\n- host: www.farmersinsurance.com\n  https: true\n  tls_cert_error: >-\n    [SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate\n    is not valid for 'www.farmersinsurance.com'\
  \ (served cert CN=a248.e.akamai.net)\n  hsts: null\ndomains:\n- domain: farmers.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:%{ir}.%{v}.%{d}.spf.has.pphosted.com -all\n  dmarc: true\n  dmarc_policy: reject\n- domain: farmersinsurance.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:%{ir}.%{v}.%{d}.spf.has.pphosted.com ~all\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/farmers-insurance-exchange/refs/heads/main/security/farmers-insurance-exchange-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 500
- Insurance
- Property and Casualty
- Auto Insurance
- Home Insurance
- Financial Services
- United States
---
