---
title: Overview
---

# Buttons

> Buttons allow an application to communicate action and direct user intent.

## Three different types

Clarity comes with three different types of buttons to use. They are provided to give visual distinction between the priority or heirarchy of the buttons in the application.

<ClrRow>
<ClrCell>
<ClrInset><button class="btn btn-primary">Solid Button</button></ClrInset>

Solid buttons look heavy on purpose. They direct the user’s attention to the **primary action** the application is suggesting that the user take.

</ClrCell>
<ClrCell>
<ClrInset><button class="btn">Outline Button</button></ClrInset>

Outline buttons provide a lighter weight button style. They are used to indicate a **secondary action** that compliments a primary action or to reduce visual noise when there are many action of **equal** importance on the page.

</ClrCell>
<ClrCell>
<ClrInset><button class="btn btn-link">Flat Button</button></ClrInset>

Flat buttons are used in multiple scenarios. They are used as **tertiary buttons**. They can also be used inline because they are different from content in style and recognizable as buttons alongside content.

</ClrCell>
</ClrRow>

## Buttons vs Links

While buttons and links can both be given similar visual treatments, it is important that you use a link (or anchor element) for anytime clicking the element will _navigate_ you to a different page. Buttons are for interaction in the current page, such as refreshing the content or submitting a form.

<ClrRow>
<ClrCell>
<ClrInset><button class="btn btn-link">Flat Button</button></ClrInset>

Use flat buttons when a user is expected to **take an action**.

</ClrCell>

<ClrCell>
<ClrInset><a href="javascript://" class="btn btn-link">Anchor Link</a></ClrInset>

Use a link when a user is expected to be **taken to a different page**.

</ClrCell>
</ClrRow>

## Placement

There are two distinct patterns when it comes to the placement of a button.

<ClrRow>
<ClrCell>
<ClrInset height="300">
<ClrImage title="Z Pattern illustration" src="/images/components/button/z_pattern.svg" />
</ClrInset>

**Z Pattern**

The Z-pattern is a natural way for the user to go through content within a **constrained container** and when tasks are oriented from the top-left and ending with a **primary call to action on the right bottom side** of the container. This pattern is reversed for right to left languages.

<cds-icon shape="bookmark"></cds-icon> Modals and Wizards follow the Z Pattern

</ClrCell>

<ClrCell>
<ClrInset height="300">
<ClrImage title="F Pattern illustration" src="/images/components/button/f_pattern.svg" />
</ClrInset>

**F Pattern**

The F-pattern is a natural way to go through content in an **unconstrained container**, such as a form on the page itself. The user will go through the content line-by-line, arriving at a call to action at the end.

<cds-icon shape="bookmark"></cds-icon> Forms and Cards follow the F Pattern

</ClrCell>
</ClrRow>

## Style

Consistent button styles make it easier for a user to recognize areas to take action across an application.

### Typography

The text inside of buttons is always **uppercase**. This indicates action by differentiating button text from links and other content on the page. Use descriptive language on buttons relating to the user’s intent.

<ClrRow>
<ClrCell>
<ClrDoDont>
<template v-slot:demo>
<ClrImage title="Typography Don Example" src="/images/components/button/typography_do.svg" />
</template>
<template v-slot:summary>
Use a call to action on buttons.
</template>
</ClrDoDont>
</ClrCell>
<ClrCell>
<ClrDoDont dont>
<template v-slot:demo>
<ClrImage title="Typography Don't Example" src="/images/components/button/typography_dont.svg" />
</template>
<template v-slot:summary>
Use generic language not related to the action and not relating to the intent of the user.
</template>
</ClrDoDont>
</ClrCell>
</ClrRow>

### Visual Style

Clarity buttons have several distinct properties and design considerations.

#### Border Radius

Clarity buttons have a border radius of 3px.

<ClrRow>
<ClrCell>

#### Size

Clarity offers two button sizes:

* Default height of 36px
* Compact height of 24px

Compact is used in content areas where smaller buttons are needed to de-emphasize calls to action. This is especially true when multiple actions of equal importance are available.

</ClrCell>
<ClrCell>

<ClrImage title="Visualization of button sizes" src="/images/components/button/button_sizes.png" />

</ClrCell>
</ClrRow>

<ClrRow>
<ClrCell>

#### Primary Color

A primary color provides consistency across an application. It trains the user to look for that color when trying to find an action. Clarity defaults to blue. This “action blue” can be found across all types of buttons, tabs, and other action-related components.

</ClrCell>
<ClrCell />
</ClrRow>

<ClrRow>
<ClrCell>

#### Action-based Color

Different colors may be used based on the severity of an action’s result. For example, using a red button when “deleting” files indicates high severity.

</ClrCell>
<ClrCell>
<ClrImage title="Visualization of button colors" src="/images/components/button/action_colors.png" />
</ClrCell>
</ClrRow>

## Icons

Icon buttons are useful where interface space may be limited. If an icon represents the action well, users can sometimes recognize them quicker than reading text. Lastly, using icon buttons can help in the situation where the use of long labels may be challenging.

We recommend you **choose an icon that best describes the action** that the user will be doing. Users may avoid unknown or abstract icon buttons.

### Types & Sizes

<ClientOnly>
<ClrRow>
<ClrCell>
<ClrDoDont demoHeight="100">
<template v-slot:demo>
<cds-button size="icon" style="margin-right: 12px"><cds-icon shape="check"></cds-icon></cds-button>
<cds-button size="icon" action="outline" style="margin-right: 12px"><cds-icon shape="folder"></cds-icon></cds-button>
<cds-button size="icon" action="flat"><cds-icon shape="cog"></cds-icon></cds-button>
</template>
<template v-slot:summary>
Icon buttons are available in the solid, outline, and flat types. It’s also best to use the normal (36px) sized ones. This makes them easier to recognize and to click.
</template>
</ClrDoDont>
</ClrCell>
<ClrCell>
<ClrDoDont dont demoHeight="100">
<template v-slot:demo>
<cds-button size="sm" style="margin-right: 12px"><cds-icon shape="check"></cds-icon></cds-button>
<cds-button size="sm" action="outline" style="margin-right: 12px"><cds-icon shape="folder"></cds-icon></cds-button>
<cds-button size="sm" action="flat"><cds-icon shape="cog"></cds-icon></cds-button>
</template>
<template v-slot:summary>
Use small icon buttons in most cases. They are difficult to see and distinguish what the icon is or represents. They also create smaller click targets, making them harder to click.
</template>
</ClrDoDont>
</ClrCell>
</ClrRow>
</ClientOnly>

### With Text

<ClientOnly>
<ClrRow>
<ClrCell>
<ClrDoDont demoHeight="100">
<template v-slot:demo>
<cds-button size="icon" style="margin-right: 12px"><cds-icon shape="check"></cds-icon> Create</cds-button>
<cds-button size="icon" action="outline"><cds-icon shape="times"></cds-icon> Delete</cds-button>
</template>
<template v-slot:summary>
If you have the space, adding text helps users understand the action. Start icon buttons with icons and follow with text.
</template>
</ClrDoDont>
</ClrCell>
<ClrCell>
<ClrDoDont dont demoHeight="100">
<template v-slot:demo>
<cds-button size="icon" style="margin-right: 12px">Create <cds-icon shape="check"></cds-icon></cds-button>
<cds-button size="icon" action="outline">Delete <cds-icon shape="times"></cds-icon></cds-button>
</template>
<template v-slot:summary>
Start icon buttons with text and follow with icon. This makes them more difficult to scan quickly.
</template>
</ClrDoDont>
</ClrCell>
</ClrRow>
</ClientOnly>

<ClrRow>
<ClrCell>

### Title Attribute

If your icon button is has no text, we recommend adding the `title=""` attribute to your icon buttons. This adds some additional context for users unfamiliar with what action your icon button might produce. Hovering over the icon button for a moment will show a tooltip that has the `title` text. The text should reflect the action being completed.

</ClrCell>
<ClrCell>

<ClrImage title="Visualization of button title attributes" src="/images/components/button/icon-button-title-attribute.png" />

</ClrCell>
</ClrRow>