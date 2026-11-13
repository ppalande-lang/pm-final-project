# Mindmap: Daily Water Intake App

A PM view of a mobile hydration tracker, organized around three questions: **what do users need**, **what do we build to meet those needs**, and **what could go wrong**.

```mermaid
mindmap
  root((Daily Water<br/>Intake App))
    User Needs
      Know how much to drink
        Goal that fits my body
        Goal that adapts to heat and exercise
        Trustworthy, not made-up advice
      Remember to drink
        Nudges at the right moment
        No nagging during meetings or sleep
      Log with near-zero effort
        Under 3 seconds per entry
        Log without opening the app
        Fix mistakes easily
      Stay motivated
        See progress today
        Feel a sense of achievement
        Recover after a missed day
      Understand impact
        Am I improving over time
        Link to energy, sleep, headaches
      Feel in control of my data
        Private health information
        Export or delete anytime
      Special contexts
        Pregnancy and nursing
        Older adults with low thirst
        Athletes and heavy sweaters
        Medically advised intake limits
    Features
      Onboarding
        Personalized goal from weight, age, activity
        Goal explained in plain language
        Optional health permissions
      Logging
        One-tap preset cups
        Custom bottle sizes
        Home and lock screen widgets
        Smartwatch app
        Voice logging via Siri or Assistant
        Undo and edit history
      Drink types
        Water, tea, coffee, juice
        Hydration factor per drink
        Caffeine and sugar notes
      Reminders
        Smart timing based on pace
        Quiet hours and calendar aware
        Snooze and frequency control
      Progress
        Daily fill visual
        Weekly and monthly trends
        Streaks with grace days
        Badges and milestones
      Insights
        Best and worst times of day
        Weather and workout adjustments
        Shareable report for a doctor
      Integrations
        Apple Health and Google Fit
        Wearables for activity data
        Smart bottles for auto logging
        Weather API
      Social
        Friend and family challenges
        Workplace wellness teams
      Privacy controls
        Local first storage option
        Data export and account deletion
    Potential Problems
      User problems
        Forgets to log, not to drink
        Data becomes inaccurate, trust drops
        Reminder fatigue leads to muting or uninstall
        Novelty fades after week 1 to 2
        Streak loss feels punishing and causes churn
        Guessing cup sizes is error prone
      Product problems
        One size goals feel wrong
        Gamification can feel childish for some users
        Too many features clutter a simple job
        Hard to show real health value
      Health and safety
        Over-hydration risk, hyponatremia
        Users with kidney or heart conditions
        App treated as medical advice
        Encouraging obsessive tracking
      Technical problems
        OS limits on background notifications
        Health sync conflicts and duplicate logs
        Widget and watch reliability
        Smart bottle pairing and battery issues
      Business problems
        Crowded, commoditized market
        Low willingness to pay
        Low switching cost to free apps
        Retention depends on habit, hard to build
      Legal and privacy
        Health data rules, GDPR and HIPAA where applicable
        App store health claim policies
        Consent for minors
```

## Needs → Features → Risks

How the three branches connect. Each core need maps to the feature that addresses it and the main risk to watch.

| User need | Key feature(s) | Main risk | Mitigation |
|---|---|---|---|
| Know how much to drink | Personalized, adaptive goal | Goal feels arbitrary or unsafe | Show the "why"; cap goals; medical disclaimer and override |
| Remember to drink | Smart, calendar-aware reminders | Reminder fatigue → uninstall | Adaptive frequency, easy snooze, quiet hours by default |
| Log with zero effort | Widgets, watch, voice, presets | Missed logs → bad data → lost trust | Lock screen logging; "catch-up" prompt at end of day |
| Stay motivated | Fill visual, streaks, badges | Streak loss causes churn | Grace days and streak repair; celebrate weekly consistency |
| Understand impact | Trends and correlations | Weak or misleading insights | Only show insights with enough data; avoid health claims |
| Control my data | Privacy settings, export, delete | Health data breach or misuse | Data minimization, local-first option, clear consent |

## MVP scope suggestion

- **In:** personalized goal, one-tap logging + widget, smart reminders with quiet hours, daily progress + streaks with grace days, Apple Health / Google Fit sync.
- **Later:** drink-type hydration factors, insights, social challenges, smart bottles, doctor reports.
- **Riskiest assumption to test first:** users will keep logging past week 2 if logging takes under 3 seconds and reminders adapt to their pace.
