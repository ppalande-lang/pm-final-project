# Strategic Discovery Map (Module 1)

## Responses
- **Write one feature from the map that, if an engineer asked “why is this a priority for our 12-week roadmap?”, you honestly could not give a strategic answer for.:** Smart bottle integration

A smart bottle has sensors in its cap or base that measure how much water you drink. With this feature, the bottle sends that data to our app automatically, so users don’t log anything by hand. Examples on the market are HidrateSpark, LARQ and REBO.

Value vs. cost

Benefits:

Logging takes no effort for users who own a bottle.
Data is more accurate than people remembering what they drank.
It could earn money through bottle partnerships, such as a bottle bundled with a premium subscription.

Costs and limits:

Only users who buy hardware benefit, likely a small share.
It depends on outside companies’ firmware, APIs and release schedules.
It adds ongoing support and QA work for every bottle model.
It doesn’t fix the main reason people quit, which is lost motivation, not effort.
- **Write one feature that looks “correct” for the app but has zero strategic weight, you have no idea if it helps the company make money or whether a single user actually asked for it.:** Weather-adjusted daily goal: the app checks the local forecast each morning and raises the goal on hot or humid days (for example, +250 ml above 30°C).

Why it looks correct

It sounds smart and personal, and it’s easy to demo.
It makes sense physiologically, since people do lose more water in the heat.
It fits the product story of a goal that adapts to you, and I put it in the mindmap myself under Features and Insights without questioning it.
It’s simple to build: one weather API call and a formula.

Why it has no strategic weight

No user asked for it. Nothing in the user needs points to it. The pain points we listed are forgetting to drink, logging taking too long and motivation fading. Nobody said “my goal is wrong on hot days.”
It doesn’t touch the riskiest assumption. We said the real bet is whether people keep logging past week 2. A changing goal does nothing for logging effort, and it may hurt motivation: a target that keeps moving can feel like the app is cheating you out of your streak.
It doesn’t connect to revenue. It’s not a reason to upgrade to premium, it doesn’t help with corporate wellness sales, and it doesn’t make the app harder to leave. Any competitor can copy it in a sprint.
We can’t measure its impact. Hot days are rare and seasonal, and they vary by region. Even with an A/B test, it would take a long time to see any effect on retention.
It adds risk. It’s a health-related claim that needs a review for liability, and it brings in a dependency on an outside weather service.

What would give it weight

I’d keep it off the roadmap until one of these is true:

Interviews or support tickets show users manually changing their goal on hot days.
Data shows missed goals cluster on hot days and lead to people quitting.
A paying segment (outdoor workers, athletes, corporate wellness buyers in hot climates) says it would help them choose us.
- **Compare V3 to your Step 1 baseline. What changed, and is the output objectively better, did the AI get smarter, or did your added PM knowledge (JTBD, effort/impact, retention) force it to be useful?:** My Step 1 baseline was a generic feature list: users, problems, features and metrics, with every idea given equal weight and no guidance on what to do first. In V3 I gave the prompt PM structure: jobs-to-be-done, friction points, features sorted by effort and impact, monetization tradeoffs, retention risks, and an instruction to flag strategic tensions.

Each addition changed the output in a specific way:

JTBD showed that water is the means, not the goal. Users really want to feel less tired, which raised the question of whether we're building a reminder app or an outcome app.
Effort vs. impact turned the feature list into an MVP (one-tap widget logging, context-aware reminders, grace days) and an "avoid for now" list.
Retention risks surfaced the problem that users who build the habit may stop needing the app.
Flagging tensions turned the output into debates the team has to settle, such as engagement metrics vs. an app users barely need to open.

So yes, V3 is better, but the AI didn't get smarter. The same model produced a better answer because the prompt carried better thinking. The improvement came from my PM frameworks, not from the AI.
- **Key takeaway: how does this prove the PM’s role is to think while the AI’s role is to execute?:** The AI produced the smart bottle integration and the weather-adjusted goal with confident, reasonable-sounding justifications. It took my judgment to see that neither addresses the riskiest assumption (whether people keep logging past week 2), neither is backed by a user request, and neither connects to revenue. The AI can generate and organize options quickly, but it can't tell which ones matter. The PM's job is to frame the problem, ask the right questions, and decide what earns a place on the roadmap. The AI then executes on that framing.
