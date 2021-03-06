# `harness.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test internal/compiler/lint/rules/harness.test.ts --update-snapshots` to update.

## `react/noDangerWithChildren`

### `0`

```

 lint/react/noDangerWithChildren/reject/1/file.tsx:1 lint/react/noDangerWithChildren ━━━━━━━━━━━━━━━

  ✖ Avoid passing both children and the dangerouslySetInnerHTML prop.

    <div dangerouslySetInnerHTML={{ __html: 'HTML' }}>children</div>
    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

  ℹ Setting HTML content will inadvertently override any passed children in React.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```

### `0: formatted`

```
<div dangerouslySetInnerHTML={{__html: "HTML"}}>
	children
</div>;

```

### `1`

```

 lint/react/noDangerWithChildren/reject/2/file.tsx:1 lint/react/noDangerWithChildren ━━━━━━━━━━━━━━━

  ✖ Avoid passing both children and the dangerouslySetInnerHTML prop.

    <div dangerouslySetInnerHTML={{ __html: 'HTML' }} children={'children'} />
    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

  ℹ Setting HTML content will inadvertently override any passed children in React.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```

### `1: formatted`

```
<div dangerouslySetInnerHTML={{__html: "HTML"}} children={"children"} />;

```

### `2`

```

 lint/react/noDangerWithChildren/reject/3/file.tsx:1 lint/react/noDangerWithChildren ━━━━━━━━━━━━━━━

  ✖ Avoid passing both children and the dangerouslySetInnerHTML prop.

    <div dangerouslySetInnerHTML={{ __html: 'HTML' }} children={['children']} />
    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

  ℹ Setting HTML content will inadvertently override any passed children in React.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```

### `2: formatted`

```
<div dangerouslySetInnerHTML={{__html: "HTML"}} children={["children"]} />;

```

### `3`

```

 lint/react/noDangerWithChildren/reject/4/file.tsx:1 lint/react/noDangerWithChildren ━━━━━━━━━━━━━━━

  ✖ Avoid passing both children and the dangerouslySetInnerHTML prop.

    <Invalid dangerouslySetInnerHTML={{ __html: 'HTML' }}>children</Invalid>
    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

  ℹ Setting HTML content will inadvertently override any passed children in React.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```

### `3: formatted`

```
<Invalid dangerouslySetInnerHTML={{__html: "HTML"}}>
	children
</Invalid>;

```

### `4`

```

 lint/react/noDangerWithChildren/reject/5/file.tsx:1 lint/react/noDangerWithChildren ━━━━━━━━━━━━━━━

  ✖ Avoid passing both children and the dangerouslySetInnerHTML prop.

    <Invalid dangerouslySetInnerHTML={{ __html: 'HTML' }} children={'children'}/>
    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

  ℹ Setting HTML content will inadvertently override any passed children in React.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```

### `4: formatted`

```
<Invalid dangerouslySetInnerHTML={{__html: "HTML"}} children={"children"} />;

```

### `5`

```

 lint/react/noDangerWithChildren/reject/6/file.tsx:1 lint/react/noDangerWithChildren ━━━━━━━━━━━━━━━

  ✖ Avoid passing both children and the dangerouslySetInnerHTML prop.

    React.createElement('div', { dangerouslySetInnerHTML: { __html: 'HTML' } }, 'children')
    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

  ℹ Setting HTML content will inadvertently override any passed children in React.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```

### `5: formatted`

```
React.createElement(
	"div",
	{dangerouslySetInnerHTML: {__html: "HTML"}},
	"children",
);

```

### `6`

```

 lint/react/noDangerWithChildren/reject/7/file.tsx:1 lint/react/noDangerWithChildren ━━━━━━━━━━━━━━━

  ✖ Avoid passing both children and the dangerouslySetInnerHTML prop.

    React.createElement('div', { dangerouslySetInnerHTML: { __html: 'HTML' } }, ['children'])
    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

  ℹ Setting HTML content will inadvertently override any passed children in React.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```

### `6: formatted`

```
React.createElement(
	"div",
	{dangerouslySetInnerHTML: {__html: "HTML"}},
	["children"],
);

```

### `7`

```

 lint/react/noDangerWithChildren/reject/8/file.tsx:1 lint/react/noDangerWithChildren ━━━━━━━━━━━━━━━

  ✖ Avoid passing both children and the dangerouslySetInnerHTML prop.

    React.createElement('div', { dangerouslySetInnerHTML: { __html: 'HTML' }, children: 'children'
       })
    ^^^^^^^^^^^

  ℹ Setting HTML content will inadvertently override any passed children in React.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```

### `7: formatted`

```
React.createElement(
	"div",
	{dangerouslySetInnerHTML: {__html: "HTML"}, children: "children"},
);

```

### `8`

```

 lint/react/noDangerWithChildren/reject/9/file.tsx:1 lint/react/noDangerWithChildren ━━━━━━━━━━━━━━━

  ✖ Avoid passing both children and the dangerouslySetInnerHTML prop.

    React.createElement('div', { dangerouslySetInnerHTML: { __html: 'HTML' }, children:
    ['children'] })
    ^^^^^^^^^^^^^^^^^^^^^^

  ℹ Setting HTML content will inadvertently override any passed children in React.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```

### `8: formatted`

```
React.createElement(
	"div",
	{dangerouslySetInnerHTML: {__html: "HTML"}, children: ["children"]},
);

```

### `9`

```

 lint/react/noDangerWithChildren/reject/10/file.tsx:1 lint/react/noDangerWithChildren ━━━━━━━━━━━━━━

  ✖ Avoid passing both children and the dangerouslySetInnerHTML prop.

    React.createElement('Invalid', { dangerouslySetInnerHTML: { __html: 'HTML' }, children:
    'children' })
    ^^^^^^^^^^^^^^^^^^^^

  ℹ Setting HTML content will inadvertently override any passed children in React.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```

### `9: formatted`

```
React.createElement(
	"Invalid",
	{dangerouslySetInnerHTML: {__html: "HTML"}, children: "children"},
);

```

### `10`

```

 lint/react/noDangerWithChildren/reject/11/file.tsx:1 lint/react/noDangerWithChildren ━━━━━━━━━━━━━━

  ✖ Avoid passing both children and the dangerouslySetInnerHTML prop.

    React.createElement('Invalid', { dangerouslySetInnerHTML: { __html: 'HTML' }, children:
    ['children'] })
    ^^^^^^^^^^^^^^^^^^^^^^

  ℹ Setting HTML content will inadvertently override any passed children in React.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```

### `10: formatted`

```
React.createElement(
	"Invalid",
	{dangerouslySetInnerHTML: {__html: "HTML"}, children: ["children"]},
);

```

### `11`

```

 lint/react/noDangerWithChildren/reject/12/file.tsx:1 lint/react/noDangerWithChildren ━━━━━━━━━━━━━━

  ✖ Avoid passing both children and the dangerouslySetInnerHTML prop.

    React.createElement('Invalid', { dangerouslySetInnerHTML: { __html: 'HTML' } }, 'children')
    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

  ℹ Setting HTML content will inadvertently override any passed children in React.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```

### `11: formatted`

```
React.createElement(
	"Invalid",
	{dangerouslySetInnerHTML: {__html: "HTML"}},
	"children",
);

```

### `12`

```

 lint/react/noDangerWithChildren/reject/13/file.tsx:1 lint/react/noDangerWithChildren ━━━━━━━━━━━━━━

  ✖ Avoid passing both children and the dangerouslySetInnerHTML prop.

    React.createElement('Invalid', { dangerouslySetInnerHTML: { __html: 'HTML' } }, ['children'])
    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

  ℹ Setting HTML content will inadvertently override any passed children in React.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```

### `12: formatted`

```
React.createElement(
	"Invalid",
	{dangerouslySetInnerHTML: {__html: "HTML"}},
	["children"],
);

```

### `13`

```

 lint/react/noDangerWithChildren/reject/14/file.tsx:1 lint/react/noDangerWithChildren ━━━━━━━━━━━━━━

  ✖ Avoid passing both children and the dangerouslySetInnerHTML prop.

    createElement('div', { dangerouslySetInnerHTML: { __html: 'HTML' } }, 'children')
    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

  ℹ Setting HTML content will inadvertently override any passed children in React.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```

### `13: formatted`

```
createElement("div", {dangerouslySetInnerHTML: {__html: "HTML"}}, "children");

```

### `14`

```

 lint/react/noDangerWithChildren/reject/15/file.tsx:1 lint/react/noDangerWithChildren ━━━━━━━━━━━━━━

  ✖ Avoid passing both children and the dangerouslySetInnerHTML prop.

    createElement('div', { dangerouslySetInnerHTML: { __html: 'HTML' } }, ['children'])
    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

  ℹ Setting HTML content will inadvertently override any passed children in React.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```

### `14: formatted`

```
createElement("div", {dangerouslySetInnerHTML: {__html: "HTML"}}, ["children"]);

```

### `15`

```

 lint/react/noDangerWithChildren/reject/16/file.tsx:1 lint/react/noDangerWithChildren ━━━━━━━━━━━━━━

  ✖ Avoid passing both children and the dangerouslySetInnerHTML prop.

    createElement('div', { dangerouslySetInnerHTML: { __html: 'HTML' }, children: 'children' })
    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

  ℹ Setting HTML content will inadvertently override any passed children in React.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```

### `15: formatted`

```
createElement(
	"div",
	{dangerouslySetInnerHTML: {__html: "HTML"}, children: "children"},
);

```

### `16`

```

 lint/react/noDangerWithChildren/reject/17/file.tsx:1 lint/react/noDangerWithChildren ━━━━━━━━━━━━━━

  ✖ Avoid passing both children and the dangerouslySetInnerHTML prop.

    createElement('div', { dangerouslySetInnerHTML: { __html: 'HTML' }, children: ['children'] })
    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

  ℹ Setting HTML content will inadvertently override any passed children in React.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```

### `16: formatted`

```
createElement(
	"div",
	{dangerouslySetInnerHTML: {__html: "HTML"}, children: ["children"]},
);

```

### `17`

```

 lint/react/noDangerWithChildren/reject/18/file.tsx:1 lint/react/noDangerWithChildren ━━━━━━━━━━━━━━

  ✖ Avoid passing both children and the dangerouslySetInnerHTML prop.

    createElement('Invalid', { dangerouslySetInnerHTML: { __html: 'HTML' }, children: 'children'
    })
    ^^^^^^^^^^

  ℹ Setting HTML content will inadvertently override any passed children in React.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```

### `17: formatted`

```
createElement(
	"Invalid",
	{dangerouslySetInnerHTML: {__html: "HTML"}, children: "children"},
);

```

### `18`

```

 lint/react/noDangerWithChildren/reject/19/file.tsx:1 lint/react/noDangerWithChildren ━━━━━━━━━━━━━━

  ✖ Avoid passing both children and the dangerouslySetInnerHTML prop.

    createElement('Invalid', { dangerouslySetInnerHTML: { __html: 'HTML' }, children: ['children']
       })
    ^^^^^^^^^^^

  ℹ Setting HTML content will inadvertently override any passed children in React.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```

### `18: formatted`

```
createElement(
	"Invalid",
	{dangerouslySetInnerHTML: {__html: "HTML"}, children: ["children"]},
);

```

### `19`

```

 lint/react/noDangerWithChildren/reject/20/file.tsx:1 lint/react/noDangerWithChildren ━━━━━━━━━━━━━━

  ✖ Avoid passing both children and the dangerouslySetInnerHTML prop.

    createElement('Invalid', { dangerouslySetInnerHTML: { __html: 'HTML' } }, 'children')
    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

  ℹ Setting HTML content will inadvertently override any passed children in React.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```

### `19: formatted`

```
createElement(
	"Invalid",
	{dangerouslySetInnerHTML: {__html: "HTML"}},
	"children",
);

```

### `20`

```

 lint/react/noDangerWithChildren/reject/21/file.tsx:1 lint/react/noDangerWithChildren ━━━━━━━━━━━━━━

  ✖ Avoid passing both children and the dangerouslySetInnerHTML prop.

    createElement('Invalid', { dangerouslySetInnerHTML: { __html: 'HTML' } }, ['children'])
    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

  ℹ Setting HTML content will inadvertently override any passed children in React.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```

### `20: formatted`

```
createElement(
	"Invalid",
	{dangerouslySetInnerHTML: {__html: "HTML"}},
	["children"],
);

```

### `21`

```
✔ No known problems!

```

### `21: formatted`

```
<div dangerouslySetInnerHTML={{__html: "HTML"}} />;

```

### `22`

```
✔ No known problems!

```

### `22: formatted`

```
<div>
	children
</div>;

```

### `23`

```
✔ No known problems!

```

### `23: formatted`

```
<div children={"children"} />;

```

### `24`

```
✔ No known problems!

```

### `24: formatted`

```
<div children={["children"]} />;

```

### `25`

```
✔ No known problems!

```

### `25: formatted`

```
<Valid dangerouslySetInnerHTML={{__html: "HTML"}} />;

```

### `26`

```
✔ No known problems!

```

### `26: formatted`

```
<Valid>
	children
</Valid>;

```

### `27`

```
✔ No known problems!

```

### `27: formatted`

```
<Valid children={"children"} />;

```

### `28`

```
✔ No known problems!

```

### `28: formatted`

```
<Valid children={["children"]} />;

```

### `29`

```
✔ No known problems!

```

### `29: formatted`

```
React.createElement("div", {dangerouslySetInnerHTML: {__html: "HTML"}});

```

### `30`

```
✔ No known problems!

```

### `30: formatted`

```
React.createElement("div", {}, "children");

```

### `31`

```
✔ No known problems!

```

### `31: formatted`

```
React.createElement("div", {}, ["children"]);

```

### `32`

```
✔ No known problems!

```

### `32: formatted`

```
React.createElement("div", {children: "children"});

```

### `33`

```
✔ No known problems!

```

### `33: formatted`

```
React.createElement("div", {children: ["children"]});

```

### `34`

```
✔ No known problems!

```

### `34: formatted`

```
React.createElement("valid", {dangerouslySetInnerHTML: {__html: "HTML"}});

```

### `35`

```
✔ No known problems!

```

### `35: formatted`

```
React.createElement("valid", {}, "children");

```

### `36`

```
✔ No known problems!

```

### `36: formatted`

```
React.createElement("valid", {}, ["children"]);

```

### `37`

```
✔ No known problems!

```

### `37: formatted`

```
React.createElement("valid", {children: "children"});

```

### `38`

```
✔ No known problems!

```

### `38: formatted`

```
React.createElement("valid", {children: ["children"]});

```

### `39`

```
✔ No known problems!

```

### `39: formatted`

```
createElement("div", {dangerouslySetInnerHTML: {__html: "HTML"}});

```

### `40`

```
✔ No known problems!

```

### `40: formatted`

```
createElement("div", {}, "children");

```

### `41`

```
✔ No known problems!

```

### `41: formatted`

```
createElement("div", {}, ["children"]);

```

### `42`

```
✔ No known problems!

```

### `42: formatted`

```
createElement("div", {children: "children"});

```

### `43`

```
✔ No known problems!

```

### `43: formatted`

```
createElement("div", {children: ["children"]});

```

### `44`

```
✔ No known problems!

```

### `44: formatted`

```
createElement("valid", {dangerouslySetInnerHTML: {__html: "HTML"}});

```

### `45`

```
✔ No known problems!

```

### `45: formatted`

```
createElement("valid", {}, "children");

```

### `46`

```
✔ No known problems!

```

### `46: formatted`

```
createElement("valid", {}, ["children"]);

```

### `47`

```
✔ No known problems!

```

### `47: formatted`

```
createElement("valid", {children: "children"});

```

### `48`

```
✔ No known problems!

```

### `48: formatted`

```
createElement("valid", {children: ["children"]});

```
