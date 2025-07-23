
# 📁 supabase_qms/

**Plassering:** `00_admin/02_dev_integration/supabase_qms/`  
**Kategori:** Teknisk backend for dokument- og agentlagring i QMS.

## 📐 Formål

Dette er en fullverdig Supabase-modul for håndtering av dokumenter, revisjonslogger og agentregistre i Norsains kvalitetssystem (ISO 9001). Den gir API-tilgang og frontend-integrasjon for databaserelatert funksjonalitet.

## 📦 Innhold

| Filnavn              | Beskrivelse |
|----------------------|-------------|
| `init_qms_tables.sql` | Oppretter tabeller for dokumenter, agenter og revisjonslogg |
| `qms_schema.yaml`     | Beskriver strukturen på tabellene (metadata og funksjon) |
| `.env.example`        | Eksempel på miljøvariabler brukt i utviklingsmiljøer |
| `supabaseClient.ts`   | Ferdig frontend-klientmodul for Supabase API |
| `README.md`           | Denne filen |

## 🚀 Bruk

1. Logg inn i Supabase Studio og kjør `init_qms_tables.sql` i SQL-editoren.
2. Kopier `.env.example` til `.env.local` og fyll inn prosjektets URL og nøkkel.
3. Bruk `supabaseClient.ts` i din Next.js/Vercel-applikasjon.
4. Se `README_supabase_qms.md` for detaljert bruk.

## 📚 Tillegg

- Agentstruktur kan kobles mot `agent_register.yaml` (fra `06_agenter/`)
- Dokumentversjonering skjer gjennom `revisions`-tabellen
- Fremtidige utvidelser inkluderer Supabase Edge Functions og Webhooks

