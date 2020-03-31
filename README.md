#  Indonesia-GeoJSON

JSON format of 34 Provinces of Indonesia

## How to Get Indonesia-GeoJSON Data
1. Download .shp from : **https://www.kompasiana.com/nsaripurba/5dda6c95097f364d44734282/shp-indonesia-34-provinsi**
2. Convert .shp to .geojson with : **https://qgis.org/en/site/**

## Data

|  NAME_0   |	NAME_1	          | KODE |	geometry  |
|-----------|---------------------|------|------------|
|Indonesia	|Bangka Belitung	  | 19	 |MultiPolygon|
|Indonesia	|Gorontalo	          | 75	 |MultiPolygon|
|Indonesia	|Riau	              | 14	 |MultiPolygon|
|Indonesia	|Jakarta Raya	      | 31	 |MultiPolygon|
|Indonesia	|Kepulauan Riau	      | 21	 |MultiPolygon|
|Indonesia	|Sulawesi Selatan	  | 73	 |MultiPolygon|
|Indonesia	|Sumatera Selatan	  | 16	 |MultiPolygon|
|Indonesia	|Kalimantan Barat	  | 61	 |MultiPolygon|
|Indonesia	|Aceh	              | 11	 |MultiPolygon|
|Indonesia	|Bengkulu	          | 17	 |MultiPolygon|
|Indonesia	|Lampung	          | 18	 |MultiPolygon|
|Indonesia	|Jawa Tengah		  | 33	 |MultiPolygon|
|Indonesia	|Nusa Tenggara Barat  |	52	 |MultiPolygon|
|Indonesia	|Sumatera Utara		  | 12	 |MultiPolygon|
|Indonesia	|Jambi				  | 15	 |MultiPolygon|
|Indonesia	|Banten				  | 36	 |MultiPolygon|
|Indonesia	|Jawa Timur			  | 35	 |MultiPolygon|
|Indonesia	|Yogyakarta			  | 34	 |MultiPolygon|
|Indonesia	|Kalimantan Selatan	  | 63	 |MultiPolygon|
|Indonesia	|Sulawesi Utara	      | 71	 |MultiPolygon|
|Indonesia	|Kalimantan Utara	  | 65	 |MultiPolygon|
|Indonesia	|Sulawesi Barat	      | 76	 |MultiPolygon|
|Indonesia	|Maluku Utara	      | 82	 |MultiPolygon|
|Indonesia	|Kalimantan Tengah	  | 62	 |MultiPolygon|
|Indonesia	|Nusa Tenggara Timur  |	53	 |MultiPolygon|
|Indonesia	|Papua Barat	      | 92	 |MultiPolygon|
|Indonesia	|Jawa Barat	          | 32	 |MultiPolygon|
|Indonesia	|Sulawesi Tenggara	  | 74	 |MultiPolygon|
|Indonesia	|Sumatera Barat	      | 13	 |MultiPolygon|
|Indonesia	|Papua	              | 91	 |MultiPolygon|
|Indonesia	|Kalimantan Timur	  | 64	 |MultiPolygon|
|Indonesia	|Maluku	              | 81	 |MultiPolygon|
|Indonesia	|Bali	              | 51	 |MultiPolygon|
|Indonesia	|Sulawesi Tengah	  | 72	 |MultiPolygon|

## Install in Kibana - ELK stack (sample of use)
1. Edit 'kibana.yml' in '/etc/kibana/kibana.yml'
2. add this sample configuration - (Reference from **https://www.elastic.co/guide/en/kibana/current/settings.html**)
	>map.regionmap:
	>    layers:
	> 	  - name: "Indonesian Provinces"
	> 		url: "https://raw.githubusercontent.com/arsofyan7/Indonesia-GeoJSON/master/indonesia-province.geojson"
	> 		attribution: "testes"
	>		fields:
	>		   - name: "NAME_1"
	>			 description: "Nama Provinsi"
3. Enjoy

![Sample](link-to-image)

