# 📘 README – Norsain QMS ISO 9001:2015

**Repo:** `norsain-qms-iso9001`  
**Versjon:** 0.1  
**Dato:** 2025-07-23  
**Vedlikehold:** Kvalitetsleder / Norsain Technology Group  
**Lisens:** MIT  

---

## 🎯 Formål

Dette repositoriet inneholder hele kvalitetssystemet til Norsain Technology Group, dokumentert og strukturert i henhold til **NS-EN ISO 9001:2015**. 
Det fungerer både som dokumentasjonsplattform, datakilde for Supabase, og integrasjonspunkt for AI-agenter som støtter QMS-operasjoner.

Repoet følger både ISO-struktur (kapittel 4–10) og moderne GitHub-praksis med `.md`, `.yaml`, `.sql` og `.env`-filer.

---

## 🧱 Innhold og mappestruktur

```plaintext
norsain-qms-iso9001/
├── 00_admin/                  → Metadata, intern repo-dokumentasjon
├── 01_prosesser/             → En fil per ISO 9001:2015 prosesspunkt (kap. 4–10)
├── 02_templates/             → Maler for prosedyrer, prosesser og skjema
├── 03_supabase/              → SQL og YAML for Supabase integrasjon
├── 04_docs/                  → Mermaidskjema, ISO-kart og støttefiler
├── .env.example              → Miljøvariabler for Supabase SDK-bruk
├── .gitignore                → Python-basert
├── requirements.txt          → Avhengigheter for Python-agentstøtte
├── versionslogg.yaml         → Endringslogg for prosessene
├── LICENSE                   → MIT-lisens
└── README.md                 → Dette dokumentet
```

---

## 🤖 Agent- og databaseintegrasjon

Dette QMS er utviklet for å samhandle med:

- **Supabase PostgreSQL** for lagring av prosesser og status
- **Quality Manager Agent** for utfylling, varsling og oppfølging
- **ClickUp / GitHub Projects** for prosjektstyring av ISO-arbeid

Typiske API-strukturer og datamodeller finnes i `03_supabase/`.

---

## 📦 ISO 9001-dekning

Følgende punkter fra ISO 9001:2015 dekkes av prosessfiler:

| ISO-punkt | Filnavn                         | Status      |
|-----------|----------------------------------|-------------|
| 4.1       | `qms_041_kontekst.md`           | Skjelett    |
| 4.2       | `qms_042_interessenter.md`      | Skjelett    |
| …         | …                                | …           |
| 10.3      | `qms_10x_forbedring.md`         | Skjelett    |

Se full oversikt i `01_prosesser/` eller i filen `qms_iso9001_prosesser.md`.

---

## 📋 Bruksinstruks

1. Klon repoet:
   ```bash
   git clone https://github.com/Norsain/norsain-qms-iso9001.git
   ```

2. Installer Python-avhengigheter (hvis du bruker SDK eller agenter):
   ```bash
   pip install -r requirements.txt
   ```

3. Sett opp miljøvariabler (bruk `.env.example` som mal)

4. Importer `qms_prosesser_supabase.sql` i Supabase-prosjektet ditt

---

## 🧠 Kontakt og bidrag

> Dette repoet vedlikeholdes av **Henrik Strand** / Norsain Technology Group.  
> For spørsmål: [info@norsain.com](mailto:info@norsain.com)

Bidrag, forslag og revisjonsønsker kan legges inn som Pull Requests eller Issues.

---

## 🔒 Lisens

Distribuert under [MIT-lisens](LICENSE). 
Fritt gjenbruk for kvalitetssystemer, agenter og læringsformål med kreditering.
