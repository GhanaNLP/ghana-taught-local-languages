# Ghana Taught Local Languages

The official Ghanaian local languages approved and taught in Ghanaian schools, maintained by [Ghana NLP](https://github.com/GhanaNLP).

Ghana is a multilingual nation with over 80 indigenous languages. Of these, **12 local languages** are government-sponsored and officially used as languages of instruction in basic schools across the country. In October 2025, the Ghanaian government made mother-tongue instruction compulsory at the basic school level, reinforcing the importance of these languages in education.

## Languages

| # | Language | ISO 639-3 | Est. Speakers | Family | Region |
|---|----------|-----------|---------------|--------|--------|
| 1 | Akuapem Twi | `twi` | ~2,300,000 | Kwa | Eastern |
| 2 | Asante Twi | `twi` | ~7,000,000 | Kwa | Ashanti |
| 3 | Dagaare | `dga` | ~924,000 | Gur | Upper West |
| 4 | Dagbani | `dag` | ~3,160,000 | Gur | Northern |
| 5 | Dangme | `ada` | ~1,020,000 | Kwa | Greater Accra |
| 6 | Ewe | `ewe` | ~3,820,000 | Gbe | Volta |
| 7 | Fante | `fat` | ~1,170,000 | Kwa | Central |
| 8 | Ga | `gaa` | ~745,000 | Kwa | Greater Accra |
| 9 | Gonja | `gnn` | ~310,000 | Kwa | Northern/Savannah |
| 10 | Gurene | `gur` | ~600,000 | Gur | Upper East |
| 11 | Kasem | `kas` | ~250,000 | Gur | Upper East |
| 12 | Nzema | `nzi` | ~330,000 | Kwa | Western |

> **Note:** Akuapem Twi and Asante Twi share ISO 639-3 code `twi` as varieties of Twi, which falls under the Akan macrolanguage (ISO 639-3: `aka`).

## Quick Stats

- **Total languages:** 12
- **Total estimated speakers (L1):** ~21.7 million
- **Language families represented:** 3 (Kwa, Gur, Gbe)
- **All belong to:** Niger-Congo phylum
- **Most spoken:** Asante Twi (~7M speakers)
- **Least spoken:** Kasem (~250K speakers)

## Speaker Distribution by Family

```
Kwa Languages (7)     ████████████████████████████  ~15.6M speakers
  Akuapem Twi           ~2.3M
  Asante Twi            ~7.0M
  Dangme                ~1.0M
  Fante                 ~1.2M
  Ga                    ~0.7M
  Gonja                 ~0.3M
  Nzema                 ~0.3M

Gur Languages (4)     ████████████                  ~4.9M speakers
  Dagaare               ~0.9M
  Dagbani               ~3.2M
  Gurene                ~0.6M
  Kasem                 ~0.3M

Gbe Languages (1)     ████████                      ~3.8M speakers
  Ewe                   ~3.8M
```

## Files in This Repository

| File | Description |
|------|-------------|
| `languages.csv` | CSV with language names, ISO 639-3 codes, speaker estimates, family, and region |
| `languages.json` | JSON with language names and ISO 639-3 codes |

## Usage

### CSV

```python
import csv

with open("languages.csv") as f:
    reader = csv.DictReader(f)
    for row in reader:
        print(f"{row['Language']} ({row['ISO 639-3']})")
```

### JSON

```python
import json

with open("languages.json") as f:
    data = json.load(f)
    for lang in data["languages"]:
        print(f"{lang['name']} ({lang['iso639_3']})")
```

## Background

The Bureau of Ghana Languages (BGL), established in 1951, supports these government-sponsored languages through publications and educational materials. These languages are used as mediums of instruction in basic schools, particularly during the first three years of primary education, and continue as subjects through Junior High School.

In recent years, there has been a renewed push for mother-tongue education. Research by UNESCO and the World Bank consistently shows that children learn faster and more confidently when taught in their native language, especially in early years.

## Sources

- [Languages of Ghana - Wikipedia](https://en.wikipedia.org/wiki/Languages_of_Ghana)
- [Ethnologue: Languages of Ghana](https://www.ethnologue.com/country/GH/)
- [Bureau of Ghana Languages](https://web.archive.org/web/20131112001558/http://www.ghanaculture.gov.gh/index1.php?linkid=331&page=2&sectionid=602)
- Ghana 2021 Population and Housing Census

## License

MIT
