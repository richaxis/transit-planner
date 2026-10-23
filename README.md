# Transit Planner

An open-source journey-planner API and dataset for rail and metro networks in Berlin, Paris and Madrid.

Status: early prototype built to demonstrate milestone-based grant funding.

## Purpose

Transit Planner gives developers free, documented access to stops, lines and routes in three European cities, so they can build travel apps without scraping or paying for proprietary data. The API and the dataset are both open.

## API endpoints

Base URL: `https://api.transit-planner.example/v1`

1. List supported cities

```
GET /cities
curl "https://api.transit-planner.example/v1/cities"
```

2. List stops in a city

```
GET /stops?city=berlin
curl "https://api.transit-planner.example/v1/stops?city=berlin"
```

3. Plan a journey between two stops

```
GET /routes?city=paris&from=Chatelet&to=Gare%20du%20Nord
curl "https://api.transit-planner.example/v1/routes?city=paris&from=Chatelet&to=Gare%20du%20Nord"
```

4. List lines for a city

```
GET /lines?city=madrid
curl "https://api.transit-planner.example/v1/lines?city=madrid"
```

## Installation

1. Clone the repository: `git clone https://github.com/YOUR-USERNAME/transit-planner.git`
2. Enter the folder: `cd transit-planner`
3. Install dependencies: `npm install`
4. Start the API locally: `npm start`
5. Open `http://localhost:3000/v1/cities` to check it works.

## Dataset

The dataset covers Berlin, Paris and Madrid and is available as a downloadable file: `data/transit-planner-dataset.zip` in this repository (stops, lines and routes for all three cities).

## License

The code is released under the MIT license. The dataset is released under CC-BY 4.0.
