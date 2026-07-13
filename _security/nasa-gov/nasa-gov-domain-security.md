---
api_specs:
- filename: apod-openapi.yml
  format: yaml
  label: NASA Astronomy Picture of the Day (APOD)
  slug: apod
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/apod-openapi.yml
- filename: asteroids-neows-openapi.yml
  format: yaml
  label: NASA Asteroids NeoWs (Near Earth Object Web Service)
  slug: asteroids-neows
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/asteroids-neows-openapi.yml
- filename: donki-openapi.yml
  format: yaml
  label: NASA DONKI Space Weather API
  slug: donki
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/donki-openapi.yml
- filename: earth-openapi.yml
  format: yaml
  label: NASA Earth Imagery API
  slug: earth
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/earth-openapi.yml
- filename: eonet-openapi.yml
  format: yaml
  label: NASA EONET (Earth Observatory Natural Event Tracker)
  slug: eonet
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/eonet-openapi.yml
- filename: epic-openapi.yml
  format: yaml
  label: NASA EPIC (Earth Polychromatic Imaging Camera)
  slug: epic
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/epic-openapi.yml
- filename: exoplanet-openapi.yml
  format: yaml
  label: NASA Exoplanet Archive API
  slug: exoplanet
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/exoplanet-openapi.yml
- filename: insight-openapi.yml
  format: yaml
  label: NASA InSight Mars Weather Service API
  slug: insight
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/insight-openapi.yml
- filename: mars-rover-photos-openapi.yml
  format: yaml
  label: NASA Mars Rover Photos API
  slug: mars-rover-photos
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/mars-rover-photos-openapi.yml
- filename: image-video-library-openapi.yml
  format: yaml
  label: NASA Image and Video Library API
  slug: image-video-library
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/image-video-library-openapi.yml
- filename: techtransfer-openapi.yml
  format: yaml
  label: NASA TechTransfer API
  slug: techtransfer
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/techtransfer-openapi.yml
- filename: ssd-cneos-openapi.yml
  format: yaml
  label: NASA SSD/CNEOS API
  slug: ssd-cneos
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/ssd-cneos-openapi.yml
- filename: techport-openapi.yml
  format: yaml
  label: NASA TechPort API
  slug: techport
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/techport-openapi.yml
- filename: tle-openapi.yml
  format: yaml
  label: NASA TLE API (Two-Line Element Set)
  slug: tle
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/tle-openapi.yml
- filename: satellite-situation-center-openapi.yml
  format: yaml
  label: NASA Satellite Situation Center API
  slug: satellite-situation-center
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/satellite-situation-center-openapi.yml
- filename: genelab-openapi.yml
  format: yaml
  label: NASA GeneLab Search API
  slug: genelab
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/genelab-openapi.yml
- filename: trek-wmts-openapi.yml
  format: yaml
  label: NASA Vesta/Moon/Mars Trek WMTS
  slug: trek-wmts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/openapi/trek-wmts-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nasa.gov
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: data.gov
  spf: true
hosts:
- cert_expires: Aug 31 19:21:07 2026 GMT
  host: api.nasa.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 11:13:07 2026 GMT
  host: data.nasa.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 19:11:52 2026 GMT
  host: catalog.data.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nasa Gov Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NASA Open APIs, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: NASA Open APIs
provider_slug: nasa-gov
slug: nasa-gov-domain-security
source_filename: nasa-gov-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.nasa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 19:21:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: data.nasa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 11:13:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: catalog.data.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 19:11:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nasa.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: data.gov\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nasa-gov/refs/heads/main/security/nasa-gov-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Government
- Federal
- Space
- Earth Science
- Open Data
- Astronomy
- Planetary Science
- Heliophysics
- Bioscience
- NASA
---
