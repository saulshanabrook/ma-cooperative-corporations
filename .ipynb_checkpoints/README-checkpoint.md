# MA Housing Cooperatives Corporations


Turn the list of MA housing cooperatives into a CSV so I can look for ones
with articles of incorporations as dividend shares.
Copy and paste from open cooperatives since I don't have access to their API

https://opencorporates.com/companies/us_ma?branch=&commit=Go&company_type=Housing+Co-Operative&mode=best_fields&nonprofit=&order=incorporation_date&page=8&q=&search_fields%5B%5D=name&search_fields%5B%5D=previous_names&search_fields%5B%5D=company_number&search_fields%5B%5D=other_company_numbers&utf8=%E2%9C%93

Steps:

1. Copy and paste results from each page of https://opencorporates.com/companies/us_ma?branch=&commit=Go&company_type=Housing+Co-Operative&mode=best_fields&nonprofit=&order=incorporation_date&q=&search_fields%5B%5D=name&search_fields%5B%5D=previous_names&search_fields%5B%5D=company_number&search_fields%5B%5D=other_company_numbers&utf8=%E2%9C%93
2. Use [macos-pasteboard](https://github.com/chbrown/macos-pasteboard) to paste `pbv public.html > searches/8.html`
3. Run `jupyter lab main.ipynb` to parse into `data.csv` (`conda create -c conda-forge -n ma-cooperative-corporations jupyterlab beautifulsoup4`).
4. Upload to google drive and manually go through to download articles of incorporation and scan.
