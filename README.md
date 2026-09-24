# atmajaya

A Claude skill for students of Universitas Atma Jaya Makassar (UAJM). It covers the
whole route from eligibility to the hardcover: Kuliah Kerja Profesi (KKP/magang),
the tugas akhir proposal or Ringkasan Kapasitas Diri, the skripsi, the journal
manuscript, and the seminars and sidang in between.

Every rule comes from the primary guidelines of Prodi Informatika FTI UAJM and
carries its clause number, so a student can point at the page when a supervisor asks:

| Code | Document | Edition |
|---|---|---|
| KKP | Pedoman Kuliah Kerja Profesi | 18 January 2015 |
| TA | Pedoman Penulisan Skripsi | 1 April 2015, revised 10 June 2015 |

## What it does

- **Kerangka** — a full outline for the KKP report, the proposal, the Ringkasan
  Kapasitas Diri, or the skripsi. Each required section is named the way the
  guideline names it, with what it must contain and an `[ISI: ...]` prompt for what
  the student must bring. It never invents company history, data, or citations.
- **Check** — a pre-submission checklist for each document, hard failures first.
- **Prepare** — for each seminar and the sidang: quorum, grading criteria, and the
  questions that follow from the guideline's own criteria.
- **Edge cases** — about 30 situations the guideline does not spell out (rejected
  placement, remote internship, MBKM, English-language skripsi, topic change,
  non-Informatika prodi), each answered with what the guideline says, what it does
  not say, and the safe step.

It checks eligibility first: 122 sks for KKP, 115 sks plus Tugas Mandiri dan
Seminar for the tugas akhir, IPK ≥ 2,75 for the sidang.

## Limits

- Only Prodi Informatika guidelines were read. For other UAJM programmes the
  structure is a labelled starting point and every rule is marked `[CEK]`.
- The 2015 guidelines predate MBKM, online seminars, and AI-tool policies. Where they
  are silent, the skill says so.

## Related skills

- [`pedoman`](https://github.com/bryankwandou/pedoman): format audits, plus encoded
  guidelines for eleven more Indonesian universities, five foreign institutions,
  and citation styles worldwide. Used for tesis, disertasi, and other campuses.
- [`rangka`](https://github.com/bryankwandou/rangka): outlines for any document.
- [`lugas`](https://github.com/bryankwandou/lugas): plain, specific prose.

## Install

```
git clone https://github.com/bryankwandou/atmajaya ~/.claude/skills/atmajaya
```

The guideline PDFs belong to the university and are not in this repository.

## License

MIT
