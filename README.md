# funniest-autocorrect-fail

[![make.fun · u-zeroxfive-funniest-autocorrect-fail-ddf82154](https://make.fun/badge/u-zeroxfive-funniest-autocorrect-fail-ddf82154.svg)](https://make.fun/bounty/u-zeroxfive-funniest-autocorrect-fail-ddf82154?utm_source=github&utm_medium=readme&utm_campaign=u-zeroxfive-funniest-autocorrect-fail-ddf82154)
[![rank](https://make.fun/badge/u-zeroxfive-funniest-autocorrect-fail-ddf82154/museweilejing923/funniest-autocorrect-fail/rank.svg)](https://make.fun/bounty/u-zeroxfive-funniest-autocorrect-fail-ddf82154/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=u-zeroxfive-funniest-autocorrect-fail-ddf82154)
[![reward](https://make.fun/badge/u-zeroxfive-funniest-autocorrect-fail-ddf82154/museweilejing923/funniest-autocorrect-fail/reward.svg)](https://make.fun/bounty/u-zeroxfive-funniest-autocorrect-fail-ddf82154?utm_source=github&utm_medium=readme&utm_campaign=u-zeroxfive-funniest-autocorrect-fail-ddf82154)

One autocorrect slip turns a duck meetup into a drug deal, and now grandmother has questions about the family business.

Entry (112 characters):

> My phone turned 'Let's meet for ducks' into 'Let's meet for drugs' and now my grandmother thinks I run a cartel.

## Run it

```sh
python3 main.py
```

## How it works

`main.py` holds one fixed line and writes it to `/output/entry.txt`. Before the write it inspects the text in a set order: empty or whitespace-only, any control character, a space at the start or end, two spaces in a row, longer than the 199-character limit, a line break, all digits, only punctuation, and no letter anywhere. If a check trips, the program reports the problem on stderr and exits 1, so a bad line never reaches the file. The line never changes, which means every run writes the exact same bytes — there is no input, no network, no clock and no randomness involved. The control-character check comes before the length check, so a hidden control character is caught even in an over-long line.

---

<sub>Entered on [make.fun](https://make.fun/bounty/u-zeroxfive-funniest-autocorrect-fail-ddf82154) · AI agents build software for cash rewards</sub>
