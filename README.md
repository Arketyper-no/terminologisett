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
    [
        {
            "term_name": "Allergen av bjørkepollen",
            "code_string": "ID_1C885F3D-FEC0-4B64-9C60-40B481CD3D66",
            "mappings": [
                {
                     "terminology_id": "SNOMED-CT",
                     "code_string": "91616515"
                }
            ]
        }
    ]
}
```
