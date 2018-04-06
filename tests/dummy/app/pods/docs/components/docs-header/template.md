# Docs Header

A header that gives you an easy autogenerated logo via the <code>logo</code> and <code>name</code> attributes, top-level nav, and a link to your project's versions and GitHub repo (read directly from your addon's package.json file).

{{#docs-demo as |demo|}}
  {{#demo.example name='docs-header.hbs'}}
    {{docs-header logo='ember-cli' name='Addon Docs'}}
  {{/demo.example}}

  {{demo.snippet 'docs-header.hbs'}}
{{/docs-demo}}

You can also pass in a block to render your own logo.

{{#docs-demo as |demo|}}
  {{#demo.example name='docs-header-custom-logo.hbs'}}
    {{#docs-header githubUrl='https://github.com/ember-learn/ember-cli-addon-docs'}}
      <img height='30px'
        src="/assets/images/rick-astley.jpg"
        alt="Never gonna give you up"
      />
    {{/docs-header}}
  {{/demo.example}}

  {{demo.snippet 'docs-header-custom-logo.hbs'}}
{{/docs-demo}}