# Terminologisett
Terminologisett for gjenbruk interregionalt eller regionalt.

## Navngiving
*   Språk: norsk
*   Ingen særnorske tegn (æ=ae, å=aa, ø=oe)
*   Ingen spesialtegn
*   Ingen store bokstaver.
* Skilletegn `.`
* Ordskilletegn `_`

## Interregionale

Syntax:
`land.[fagområde].løsning.[overordnet_verdisett].underordnet_verdisett`

Eksempel: `no.onk.kreftjournal.sarkom.morfologi`

## Regionale

Syntax:
`land.region.[fagområde].løsning.[overordnet_verdisett].underordnet_verdisett`

Eksempel: `no.hv.yrkesmedisin.ait.allergener`

# Verdisettfiler

## Navngiving
`[verdisettnavn].json`

## Struktur
```json
{
    "valueset_id": "no.hv.yrkesmedisin.ait.allergener", 
    "terminology_id": "FEST", # (0..1) Brukes kun når alle termer er tatt fra samme standardiserte terminologi
    "description": "Verdisett for allergener som brukes i allergen immunterapi (AIT).",
    "values": [
        {
            "preferred_term": "Bjørkepollen",
            "code_string": "ID_1C885F3D-FEC0-4B64-9C60-40B481CD3D66",
            "description": "Allergen av bjørkepollen."
            "mappings": [
                {
                    "match": ">",
                    "target": {
                        "terminology_id": "ATC",
                        "code_string": "V01A A05",
                        "preferred_term": "Trepollen"
                    }
                }
            ]
        },
        {
            "preferred_term": "Timotei",
            "code_string": "ID_FFF49EEE-F590-4AF6-9425-A15CEF3B2506",
            "description": "Allergen av timotei."
            "mappings": [
                {
                    "match": ">",
                    "target": {
                        "terminology_id": "ATC",
                        "code_string": "V01A A02",
                        "preferred_term": "Gresspollen"
                    }
                }
            ]
        }
    ]
}
```
