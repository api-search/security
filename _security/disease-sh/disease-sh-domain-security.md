---
api_specs:
- filename: disease-sh-covid-19-apple-api-openapi.yml
  format: yaml
  label: 'disease.sh COVID-19: Apple API'
  slug: disease-sh-covid-19-apple-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/disease-sh/refs/heads/main/openapi/disease-sh-covid-19-apple-api-openapi.yml
- filename: disease-sh-covid-19-government-api-openapi.yml
  format: yaml
  label: 'disease.sh COVID-19: Government API'
  slug: disease-sh-covid-19-government-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/disease-sh/refs/heads/main/openapi/disease-sh-covid-19-government-api-openapi.yml
- filename: disease-sh-covid-19-jhucsse-api-openapi.yml
  format: yaml
  label: 'disease.sh COVID-19: JHUCSSE API'
  slug: disease-sh-covid-19-jhucsse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/disease-sh/refs/heads/main/openapi/disease-sh-covid-19-jhucsse-api-openapi.yml
- filename: disease-sh-covid-19-nyt-api-openapi.yml
  format: yaml
  label: 'disease.sh COVID-19: NYT API'
  slug: disease-sh-covid-19-nyt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/disease-sh/refs/heads/main/openapi/disease-sh-covid-19-nyt-api-openapi.yml
- filename: disease-sh-covid-19-therapeutics-api-openapi.yml
  format: yaml
  label: 'disease.sh COVID-19: Therapeutics API'
  slug: disease-sh-covid-19-therapeutics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/disease-sh/refs/heads/main/openapi/disease-sh-covid-19-therapeutics-api-openapi.yml
- filename: disease-sh-covid-19-vaccine-api-openapi.yml
  format: yaml
  label: 'disease.sh COVID-19: Vaccine API'
  slug: disease-sh-covid-19-vaccine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/disease-sh/refs/heads/main/openapi/disease-sh-covid-19-vaccine-api-openapi.yml
- filename: disease-sh-covid-19-variants-api-openapi.yml
  format: yaml
  label: 'disease.sh COVID-19: Variants API'
  slug: disease-sh-covid-19-variants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/disease-sh/refs/heads/main/openapi/disease-sh-covid-19-variants-api-openapi.yml
- filename: disease-sh-covid-19-worldometers-api-openapi.yml
  format: yaml
  label: 'disease.sh COVID-19: Worldometers API'
  slug: disease-sh-covid-19-worldometers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/disease-sh/refs/heads/main/openapi/disease-sh-covid-19-worldometers-api-openapi.yml
- filename: disease-sh-influenza-cdc-api-openapi.yml
  format: yaml
  label: 'disease.sh Influenza: CDC API'
  slug: disease-sh-influenza-cdc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/disease-sh/refs/heads/main/openapi/disease-sh-influenza-cdc-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: disease.sh
  spf: true
hosts:
- cert_expires: Oct  5 05:49:02 2026 GMT
  host: disease.sh
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Disease Sh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for disease.sh, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: disease.sh
provider_slug: disease-sh
slug: disease-sh-domain-security
source_filename: disease-sh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: disease.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 05:49:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: disease.sh\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/disease-sh/refs/heads/main/security/disease-sh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- COVID-19
- Disease
- Health
- Epidemiology
- Influenza
- Vaccine
- Open Data
- Public Health
---
