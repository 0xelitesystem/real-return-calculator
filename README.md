# Real Return Calculator

See how inflation erodes purchasing power over time and what nominal return you need just to break even. The tool runs entirely in your browser and reports the nominal future value, the real value in today's dollars, what idle cash would be worth, and whether you end ahead or behind.

**Live demo:** https://0xelitesystem.github.io/real-return-calculator/

**Not financial advice.** Inflation and returns are never constant. This shows the arithmetic of the fixed rates you enter, nothing more.

## What it does

The Real Return Calculator separates the money you appear to have from the money you can actually spend. It grows your amount at the nominal return you set, then divides by cumulative inflation to express the result in today's dollars. It also tracks what the same amount left idle as cash would buy after inflation, and states the break-even return, which is simply the inflation rate.

The core idea: a portfolio that grows 6 percent while inflation runs 3.5 percent gains real ground, while idle cash loses purchasing power every year even though the dollar figure never changes.

## How to use it

1. Open `index.html` in a browser, or visit the GitHub Pages site.
2. Enter the amount today, the horizon in years, annual inflation, and your nominal return.
3. Read the receipt: nominal value, real value, idle cash value, break-even return, and the real gain or loss with an ahead or behind stamp.

## Inputs and outputs

| Input | Meaning |
| --- | --- |
| Amount today | Starting sum in today's dollars |
| Years | Length of the horizon |
| Annual inflation | Yearly rate prices rise |
| Nominal return | Yearly rate your money earns before inflation |

Outputs are the nominal end value, the inflation-adjusted real value, the eroded value of idle cash, the break-even return, and the real gain or loss.

## Method and assumptions

Nominal value is `amount * (1 + nominalReturn)^years`. Real value divides that by `(1 + inflation)^years`. Idle cash is `amount / (1 + inflation)^years`. Break-even return equals the inflation rate, the point where real value holds flat. Rates are constant and compounding is annual.

## Privacy

Runs fully client side. No analytics, no network calls, no storage.

## Related tools

- [dividend-compounding-calculator](https://github.com/0xelitesystem/dividend-compounding-calculator)
- [dca-visualizer](https://github.com/0xelitesystem/dca-visualizer)

## License

MIT. Copyright 0xelitesystem 2026.
