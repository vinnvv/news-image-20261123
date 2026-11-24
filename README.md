# Monday 23 November 2026 in one image

[![make.fun · news-image-20261123](https://make.fun/badge/news-image-20261123.svg)](https://make.fun/bounty/news-image-20261123?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261123)
[![rank](https://make.fun/badge/news-image-20261123/vinnvv/news-image-20261123/rank.svg)](https://make.fun/bounty/news-image-20261123/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261123)
[![reward](https://make.fun/badge/news-image-20261123/vinnvv/news-image-20261123/reward.svg)](https://make.fun/bounty/news-image-20261123?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261123)

A single front page that sums up Monday 23 November 2026 in seven stories,
drawn as a Swiss-modernist editorial page: cream paper, charcoal ink, and
flat crimson, navy and ochre vector scenes.

## The seven stories

1. **Ukraine, Kyiv region** - Russian strikes kill at least 15 across the
   region: 11 in a five-storey block in Dymer, 3 at a supermarket in
   Vyshneve, 1 in Bila Tserkva. Rescuers search the rubble while Zelenskyy
   urges faster Patriot deliveries.
2. **Europe** - The EU proposes its 22nd sanctions package: about 60 Russian
   banks off SWIFT, a crypto crackdown with a new task force, 70+ more
   shadow-fleet ships listed, and Russian teams barred from EU events.
   All 27 members must approve.
3. **Mediterranean** - Ukraine claims drone strikes sank a Russian corvette
   at Benghazi, Libya, and hit a cargo ship. Zelenskyy confirmed the strikes.
4. **Indonesia** - 24 confirmed dead in the PT Fonusa Agung Mulia candy
   factory fire in Cikande, Banten, with about 30 still missing.
5. **Iran, Hormuz** - Tehran vows to counter a US naval blockade of the
   Strait of Hormuz; the US Treasury sanctions 2 dozen-plus Iranian
   entities over shadow banking.
6. **Markets, Monday** - Asian tech shares fall further as the AI sell-off
   deepens; Nasdaq futures rise about 3%; euro-area inflation reads 4.0%.
7. **Science** - Anthropic says AI helped prove the Riemann hypothesis,
   raising questions over whether humans can verify the proof.

A ticker along the foot carries three more briefs: drone strikes in
Khartoum, an Amtrak derailment near Lafayette, Louisiana, and an NHS trial
of AI in breast-cancer screening.

## How it is made

`render.py` draws the whole page from scratch with Python and Pillow: every
scene is a handful of flat vector shapes, every headline and caption is set
in Liberation Sans, and the date is the largest text on the page. The page
is rendered to `entry.png` at 1024x1024.

`main.ts` is a small Node 22 program using only the standard library. It
copies `entry.png` into the output directory given by `MAKEFUN_OUTPUT_DIR`
(default `/output`), creating the directory first, and logs the file it
wrote. Running it twice produces byte-identical output.
