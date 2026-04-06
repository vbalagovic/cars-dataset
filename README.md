# CarsDataset

A comprehensive vehicle specifications database covering **cars, trucks, and motorcycles** — **35,000+ variants** across **370+ brands**.

| Dataset | Variants | Brands | Year Range | Spec Fields |
|---------|----------|--------|------------|-------------|
| Cars | 27,433 | 108 | 1898-2026 | 40+ |
| Trucks | 5,492 | 95 | 1950-2025 | 45+ |
| Motorcycles | 1,858 | 171 | 1902-2023 | 40+ |
| **Total** | **34,783** | **370+** | **1898-2026** | |

## Cars Examples

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
  "fuel_type": "gasoline",
  "engine_type": "turbocharged petrol",
  "cubic_capacity_cc": 3990,
  "cylinders": 8,
  "cylinder_config": "V",
  "power_hp": 780,
  "torque_nm": 800,
  "drive_type": "all-wheel",
  "top_speed_kmh": 340,
  "acceleration_0_100_s": "2.5"
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
  "cubic_capacity_cc": 2993,
  "cylinders": 6,
  "power_hp": 286,
  "torque_nm": 650,
  "transmission_type": "automatic",
  "gears": 8,
  "top_speed_kmh": 250,
  "fuel_consumption_combined": "4.5",
  "co2_emissions_gkm": 118,
  "price_eur": 73969,
  "features": ["ABS", "Stability Control", "LED Headlights", "...84 items"]
}
```

## Trucks Examples

### Heavy Truck — Mercedes-Benz Actros

```json
{
  "brand": "Mercedes-Benz",
  "model": "Actros",
  "variant_name": "Mercedes-Benz Actros 1845 LS",
  "trim": "1845 LS",
  "segment": "Heavy",
  "body_type": "Tractor",
  "cab_type": "Megaspace",
  "axle_config": "4x2",
  "fuel_type": "diesel",
  "cubic_capacity_cc": 12800,
  "cylinders": 6,
  "power_hp": 449,
  "torque_nm": 2200,
  "emission_standard": "Euro VI",
  "transmission_type": "automatic",
  "gears": 12,
  "gvw_kg": 18000,
  "gcw_kg": 40000,
  "fuel_tank_l": 400,
  "features": ["Engine: OM 471", "Tyres: 315/80R22.5", "...+8 more"]
}
```

### Light Truck — Volkswagen Crafter

```json
{
  "brand": "Volkswagen",
  "model": "Crafter",
  "variant_name": "VW Crafter 2.0 TDI 177",
  "segment": "Light",
  "fuel_type": "diesel",
  "cubic_capacity_cc": 1968,
  "cylinders": 4,
  "power_hp": 177,
  "torque_nm": 410,
  "emission_standard": "Euro VI",
  "gvw_kg": 5000,
  "payload_capacity_kg": 2400
}
```

## Motorcycles Examples

### Superbike — Ducati Panigale V4

```json
{
  "brand": "Ducati",
  "model": "Panigale V4",
  "year": 2022,
  "trim": "V4 S",
  "category": "sport",
  "subcategory": "supersport",
  "fuel_type": "gasoline",
  "engine_type": "Four stroke, V4, DOHC",
  "cubic_capacity_cc": 1103,
  "cylinders": 4,
  "power_hp": 214,
  "torque_nm": 124,
  "transmission_type": "manual",
  "gears": 6,
  "drive_type": "chain",
  "top_speed_kmh": 299,
  "curb_weight_kg": 195,
  "seat_height_mm": 830,
  "front_suspension": "Ohlins NIX30 43mm USD fork",
  "rear_suspension": "Ohlins TTX36 monoshock",
  "front_brake": "2x 330mm Brembo Stylema",
  "abs_type": "Bosch Cornering ABS EVO",
  "traction_control": true,
  "riding_modes": "Race, Sport, Street, Wet",
  "features": ["Quick shifter", "Wheelie control", "Launch control", "...+12 more"]
}
```

### Adventure — BMW R 1250 GS

```json
{
  "brand": "BMW",
  "model": "R 1250 GS",
  "year": 2022,
  "category": "adventure",
  "fuel_type": "gasoline",
  "engine_type": "Four stroke, boxer twin",
  "cubic_capacity_cc": 1254,
  "cylinders": 2,
  "power_hp": 136,
  "torque_nm": 143,
  "top_speed_kmh": 200,
  "curb_weight_kg": 249,
  "seat_height_mm": 850,
  "fuel_tank_capacity_l": 20.0,
  "abs_type": "BMW Motorrad ABS Pro",
  "traction_control": true,
  "riding_modes": "Rain, Road, Dynamic, Enduro"
}
```

## Cars Spec Fields

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

### Dimensions & Performance

| Field | Type | Example |
|-------|------|---------|
| `length_mm` | integer | `4963` |
| `width_mm` | integer | `1868` |
| `height_mm` | integer | `1479` |
| `wheelbase_mm` | integer | `2975` |
| `curb_weight_kg` | integer | `1735` |
| `top_speed_kmh` | integer | `250` |
| `acceleration_0_100_s` | float | `5.6` |
| `fuel_consumption_combined` | float | `4.5` (L/100km) |
| `co2_emissions_gkm` | integer | `118` |
| `price_eur` | decimal | `73969.00` |

### Features Array

Each vehicle includes an array of equipment/feature strings (avg 84 per vehicle):
```
"ABS", "Stability Control", "LED Headlights", "Navigation System",
"Adaptive Cruise Control", "Lane Keeping Assist", "Apple CarPlay", ...
```

## Truck Spec Fields

| Field | Type | Example |
|-------|------|---------|
| `segment` | string | `"Heavy"`, `"Light"` |
| `cab_type` | string | `"Megaspace"`, `"Day cab"` |
| `axle_config` | string | `"4x2"`, `"6x4"`, `"8x4"` |
| `emission_standard` | string | `"Euro VI"`, `"Euro V"` |
| `gvw_kg` | integer | `18000` |
| `gcw_kg` | integer | `40000` |
| `kerb_weight_kg` | integer | `7500` |
| `payload_capacity_kg` | integer | `10500` |
| `fuel_tank_l` | float | `400` |
| + all standard powertrain/dimension fields | | |

## Motorcycle Spec Fields

| Field | Type | Example |
|-------|------|---------|
| `category` | string | `"sport"`, `"naked"`, `"adventure"`, `"cruiser"` |
| `subcategory` | string | `"supersport"`, `"touring enduro"` |
| `seat_height_mm` | integer | `830` |
| `fuel_tank_capacity_l` | float | `16.0` |
| `front_suspension` | string | `"Ohlins NIX30 43mm USD fork"` |
| `rear_suspension` | string | `"Ohlins TTX36 monoshock"` |
| `front_brake` | string | `"2x 330mm Brembo Stylema"` |
| `rear_brake` | string | `"245mm single disc"` |
| `abs_type` | string | `"Bosch Cornering ABS EVO"` |
| `traction_control` | boolean | `true` |
| `riding_modes` | string | `"Race, Sport, Street, Wet"` |
| + all standard powertrain/dimension fields | | |

## Brand Coverage

### Cars (108 brands)
**Premium** — Audi, BMW, Mercedes-Benz, Lexus, Volvo, Jaguar, Porsche, Genesis
**Mass Market** — Toyota, Honda, Ford, Volkswagen, Hyundai, Kia, Mazda, Nissan, Subaru
**Supercar** — Ferrari, Lamborghini, McLaren, Bugatti, Pagani, Koenigsegg, Aston Martin
**Electric** — Tesla, BYD, Rivian, Polestar, Lucid, NIO, Xpeng

### Trucks (95 brands)
**European** — Mercedes-Benz, Volvo, Scania, MAN, DAF, Iveco, Renault
**Global** — Tata, Isuzu, Hino, Mitsubishi Fuso, KamAZ, Dongfeng, FAW

### Motorcycles (171 brands)
**Japanese** — Honda, Yamaha, Kawasaki, Suzuki
**European** — Ducati, BMW, KTM, Triumph, Aprilia, Husqvarna
**American** — Harley-Davidson, Indian, Zero
**Scooter** — Vespa, Piaggio, Kymco, SYM

## Sample Data

This repository contains sample data for evaluation:

### Cars
- [`vehicle_data_sample.csv`](vehicle_data_sample.csv) — 37 vehicles across 21 brands
- [`vehicle_data_sample.json`](vehicle_data_sample.json) — Same data in JSON with full feature arrays

### Trucks
- [`truck_data_sample.csv`](truck_data_sample.csv) — 30 trucks across 8 brands
- [`truck_data_sample.json`](truck_data_sample.json) — Same data in JSON

### Motorcycles
- [`motorcycle_data_sample.csv`](motorcycle_data_sample.csv) — 30 motorcycles across 8 brands
- [`motorcycle_data_sample.json`](motorcycle_data_sample.json) — Same data in JSON

## Pricing

| Package | Price | Includes |
|---------|-------|----------|
| Cars Dataset | $499 one-time | 27,000+ variants, 108 brands, quarterly updates |
| Trucks Dataset | $399 one-time | 5,400+ variants, 95 brands, quarterly updates |
| Motorcycles Dataset | $299 one-time | 1,850+ variants, 171 brands, quarterly updates |
| **Complete Bundle** | **$999 one-time** | **All 3 datasets, save $198** |
| API Access | $149/month | All datasets, 5,000 req/day |

## Live Demo

Explore the dataset interactively with search, filters, and sample data:

**[autoprice-api-156269434892.europe-west1.run.app](https://autoprice-api-156269434892.europe-west1.run.app)**

## Contact

For licensing inquiries, custom exports, or API access: **greybalagovic@gmail.com**

## License

This dataset is proprietary. Sample data provided for evaluation purposes only.
