# Rhea Kulkarni

I build small, observable data pipelines. The goal is usually the same: if a batch job breaks at 3am, the next person can see why, fix it, and rerun only what failed.

## What I'm working on

- Contract-first ingestion for CSV drops that never fail silently.
- A Dagster + dbt setup where tests are part of the pipeline, not a separate chore.
- Local debugging with DuckDB so I don't need a warehouse clone for every small change.

```python
@asset
def clean_orders(rows):
    return (
        rows.drop_duplicates()
        .assign(order_date=lambda df: to_date(df["order_date"]))
    )
```

## Currently learning

How to make data contracts feel less like paperwork and more like guardrails.

![GitHub stats](https://github-readme-stats.vercel.app/api?username=gatedisclose&show_icons=true&theme=tokyonight&hide_border=true)
![Top languages](https://github-readme-stats.vercel.app/api/top-langs/?username=gatedisclose&layout=compact&theme=tokyonight&hide_border=true)