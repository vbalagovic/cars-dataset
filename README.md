# Cars Dataset

A comprehensive vehicle specifications database covering **27,000+ variants** across **108 brands** from 1898 to 2026. Each vehicle includes 40+ structured spec fields and up to 120 equipment/feature items.

| Variants | Brands | Year Range | Spec Fields | Avg Features/Vehicle |
|----------|--------|------------|-------------|----------------------|
| 27,433   | 108    | 1898-2026  | 40+         | 84                   |

## Examples

### Electric Vehicle — Tesla Model 3

```json
{
  "brand": "Tesla",
  "model": "Model 3",
  "year": 2019,
  "variant_name": "2019 Tesla Model 3 Long Range AWD specs",
  "trim": "Long Range AWD",
  "segment": "Sedan",
  "body_type": "4-doors, sedan",
  "fuel_type": "electric",
  "engine_type": "electric motor",
  "power_kw": 324,
  "power_hp": 441,
  "torque_nm": 493,
  "drive_type": "front+rear",
  "curb_weight_kg": 1831,
  "top_speed_kmh": 233,
  "acceleration_0_100_s": "4.6",
  "price_eur": 58980,
  "is_ev": true,
  "features": ["Autopilot", "Adaptive Cruise Control", "...86 items"]
}
```

### Supercar — Ferrari SF90 Spider

```json
{
  "brand": "Ferrari",
  "model": "SF90 Spider",
  "year": 2020,
  "segment": "Convertible",
  "body_type": "2 seater convertible/cabriolet",
  "fuel_type": "gasoline",
  "engine_type": "turbocharged petrol",
  "cubic_capacity_cc": 3990,
  "cylinders": 8,
  "cylinder_config": "V",
  "aspiration": "turbocharged",
  "power_kw": 573,
  "power_hp": 780,
  "torque_nm": 800,
  "drive_type": "all-wheel",
  "curb_weight_kg": 1670,
  "top_speed_kmh": 340,
  "acceleration_0_100_s": "2.5",
  "is_supercar": true
}
```

### Luxury Sedan — BMW 530d

```json
{
  "brand": "BMW",
  "model": "5 series",
  "year": 2020,
  "trim": "530d",
  "segment": "Sedan",
  "fuel_type": "diesel",
  "engine_type": "Inline 6-cylinder turbocharged diesel",
  "cubic_capacity_cc": 2993,
  "cylinders": 6,
  "cylinder_config": "Inline",
  "aspiration": "turbocharged",
  "power_hp": 286,
  "torque_nm": 650,
  "transmission_type": "automatic",
  "gears": 8,
  "drive_type": "rear",
  "top_speed_kmh": 250,
  "acceleration_0_100_s": "5.6",
  "fuel_consumption_combined": "4.5",
  "co2_emissions_gkm": 118,
  "price_eur": 73969,
  "features": ["ABS", "Stability Control", "LED Headlights", "Navigation System", "...84 items"]
}
```

### Plug-in Hybrid SUV — Ford Explorer PHEV

```json
{
  "brand": "Ford",
  "model": "Explorer",
  "year": 2020,
  "trim": "3.0 V6 EcoBoost PHEV ST-Line",
  "segment": "SUV",
  "seats": 7,
  "fuel_type": "gasoline",
  "engine_type": "plugin hybrid",
  "cylinders": 6,
  "cylinder_config": "V",
  "aspiration": "turbocharged",
  "power_hp": 457,
  "torque_nm": 825,
  "drive_type": "front+rear",
  "curb_weight_kg": 2466,
  "top_speed_kmh": 230,
  "co2_emissions_gkm": 66,
  "price_eur": 76710,
  "is_hybrid": true,
  "features": ["Adaptive Cruise Control", "Lane Keeping Assist", "...95 items"]
}
```

### Classic — 1966 Opel Rekord

```json
{
  "brand": "Opel",
  "model": "Rekord 1.5",
  "year": 1966,
  "segment": "Sedan",
  "fuel_type": "gasoline",
  "engine_type": "naturally aspirated petrol",
  "cubic_capacity_cc": 1492,
  "cylinders": 4,
  "cylinder_config": "Inline",
  "power_hp": 68,
  "torque_nm": 111,
  "transmission_type": "manual",
  "gears": 3,
  "drive_type": "rear",
  "top_speed_kmh": 135,
  "acceleration_0_100_s": "22.5"
}
```

## All Spec Fields

### Identity & Classification

| Field | Type | Example |
|-------|------|---------|
| `brand` | string | `"BMW"` |
| `model` | string | `"5 series"` |
| `year` | integer | `2020` |
| `variant_name` | string | `"2020 BMW 530d specs"` |
| `trim` | string | `"530d"` |
| `segment` | string | `"Sedan"`, `"SUV"`, `"Convertible"` |
| `body_type` | string | `"4-doors, sedan"` |
| `doors` | integer | `4` |
| `seats` | integer | `5` |

### Engine & Powertrain

| Field | Type | Example |
|-------|------|---------|
| `fuel_type` | string | `"gasoline"`, `"diesel"`, `"electric"` |
| `engine_type` | string | `"Inline 6-cylinder turbocharged diesel"` |
| `cubic_capacity_cc` | integer | `2993` |
| `cylinders` | integer | `6` |
| `cylinder_config` | string | `"Inline"`, `"V"`, `"Flat"` |
| `aspiration` | string | `"turbocharged"`, `"naturally aspirated"` |
| `power_kw` | integer | `210` |
| `power_hp` | integer | `286` |
| `torque_nm` | integer | `650` |
| `transmission_type` | string | `"automatic"`, `"manual"` |
| `gears` | integer | `8` |
| `drive_type` | string | `"rear"`, `"front"`, `"front+rear"` |

### Dimensions

| Field | Type | Example |
|-------|------|---------|
| `length_mm` | integer | `4963` |
| `width_mm` | integer | `1868` |
| `height_mm` | integer | `1479` |
| `wheelbase_mm` | integer | `2975` |
| `curb_weight_kg` | integer | `1735` |

### Performance & Consumption

| Field | Type | Example |
|-------|------|---------|
| `top_speed_kmh` | integer | `250` |
| `acceleration_0_100_s` | string | `"5.6"` |
| `fuel_consumption_combined` | string | `"4.5"` (L/100km) |
| `fuel_consumption_city` | string | `"5.8"` |
| `fuel_consumption_highway` | string | `"3.7"` |
| `co2_emissions_gkm` | integer | `118` |
| `battery_capacity_kwh` | float | `75.0` |
| `range_km` | integer | `560` |

### Pricing & Flags

| Field | Type | Example |
|-------|------|---------|
| `price_eur` | decimal | `73969.00` |
| `is_ev` | boolean | `false` |
| `is_hybrid` | boolean | `false` |
| `is_phev` | boolean | `false` |
| `is_supercar` | boolean | `false` |

### Features Array

Each vehicle includes an array of equipment and feature strings (avg 84 per vehicle). Examples:

```
"ABS", "Stability Control", "Traction Control", "LED Headlights",
"Navigation System", "Adaptive Cruise Control", "Lane Keeping Assist",
"Parking Sensors", "Heated Seats", "Leather Upholstery",
"Keyless Entry/start", "Apple CarPlay", "Android Auto", ...
```

## Brand Coverage

**Premium** — Audi, BMW, Mercedes-Benz, Lexus, Volvo, Jaguar, Land Rover, Porsche, Maserati, Genesis

**Mass Market** — Toyota, Honda, Ford, Volkswagen, Hyundai, Kia, Mazda, Nissan, Subaru, Chevrolet, Peugeot, Renault, Fiat, Skoda, SEAT

**Supercar** — Ferrari, Lamborghini, McLaren, Bugatti, Pagani, Koenigsegg, Aston Martin, Bentley, Rolls-Royce

**Electric** — Tesla, BYD, Rivian, Polestar, Lucid, NIO, Xpeng, Fisker

**Classic & Niche** — Alfa Romeo, Lancia, Saab, Studebaker, DeLorean, Morgan, Lotus, Alpine

## Sample Data

This repository contains sample data for evaluation:

- [`vehicle_data_sample.csv`](vehicle_data_sample.csv) — 37 vehicles across 21 brands
- [`vehicle_data_sample.json`](vehicle_data_sample.json) — Same data in JSON with full feature arrays

## Live API

Try the API and explore the dataset interactively:

**[autoprice-api-156269434892.europe-west1.run.app](https://autoprice-api-156269434892.europe-west1.run.app)**

## Contact

For licensing inquiries, custom exports, or API access: **greybalagovic@gmail.com**

## License

This dataset is proprietary. Sample data provided for evaluation purposes only.
