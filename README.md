#### MATS 6.0 Applicaton for Neel Nanda's Stream

[MATS 6.0 Application](https://docs.google.com/document/d/1GDFtq6PHGLlgkbCw1B7jqxwJdmK3iEPHvt_NhB_TvtQ/edit?usp=sharing) google doc summarizing my findings. I worked on finding interesting SAE features inside a 1L transformer model and reverse engineering them.

Some of the interesting features I looked at were: 

1. A `‘t` feature that is activate on the `'t` token in presence of words like don't, doesn't, etc.
2. A context dependent feature that activates on tokens ` or`, ` and` and `,` in texts are related to phone, emails, messages etc.
3. A close brackets feature? This feature activates on tokens immediately following an opening bracket `(` and boosts the logits of closing brackets `)`.
4. A relatively non-sparse feature that seems to activate on tokens that are following ` of` token. 