---
pcx-content-type: reference
title: Blocking Triggers
weight: 0
---

# Blocking Triggers

Blocking Triggers are triggers that instead of being used to define when to start an action, are used to define when to _not_ start an action. You may need to block one or more actions in a tool from firing when a specific condition arises. For these cases, you can set Blocking Triggers.

Every tool action has Firing Triggers assigned to it. Blocking Triggers are optional and, if defined, will conditionally prevent the action from starting. When you add Blocking Triggers to an action, the action will not fire if any of its Blocking Triggers are true. If the tool has more than one action, other actions without these Blocking Triggers will still work.

To conditionally block all actions in a tool, you have to configure Blocking Triggers on every action that belongs to that tool. Note that when you use Blocking Triggers, Zaraz will still load on the page.

To use Blocking Triggers, start by [creating the trigger](/zaraz/get-started/create-trigger/) with the conditions you want to use to block an event. Then:

1. Go to [Zaraz's main dashboard](https://dash.cloudflare.com/?to=/:account/:zone/zaraz).
2. Locate the third-party tool with the action you want to block and click **Edit**.
3. In **Action Name**, click the action you want to block.
4. In **Blocking Triggers**, use the dropdown menu to add a trigger to block the action.
5. Click **Save**.

{{<Aside type="note">}}

Blocking Triggers are useful if you wish to block specific actions, or even specific tools from firing, while keeping others active. If you wish to turn off Zaraz entirely on specific pages/domains/subdomains, we recommend using [Page Rules to block Zaraz](/zaraz/advanced/block-zaraz/).

{{</Aside>}}