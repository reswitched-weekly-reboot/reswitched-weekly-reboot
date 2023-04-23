{% set data = load_data(path=path) -%}
{{data | markdown | safe}}