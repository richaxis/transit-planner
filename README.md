# Transit Planner

An open-source journey-planner API for rail and metro networks in Berlin, Paris and Madrid.
Its purpose is to give developers free, documented access to European transit routes and stops.

## API endpoints

1. GET /v1/stops?city=berlin
   Example: curl "https://api.example.org/v1/stops?city=berlin"
2. GET /v1/routes?from=Alexanderplatz&to=Hauptbahnhof
   Example: curl "https://api.example.org/v1/routes?from=Alexanderplatz&to=Hauptbahnhof"
3. GET /v1/cities
   Example: curl "https://api.example.org/v1/cities"

## Installation

1. git clone https://github.com/richaxis/transit-planner
2. cd transit-planner
3. npm install
4. npm start
