# Home Assistant Blueprints

This repository is a collection of blueprints for Home Assistant.

## Available Blueprints

---

### 1. Home Location Update - Timer

* **File:** `home_loc_update_timer.yaml`
* **Description:** Periodically updates the core Home Assistant location (the one defined in `configuration.yaml`) based on the current location of a geocoded sensor.
* **Inputs:**
    * **Geocoded Location Sensor:** The sensor providing location data (e.g., from the Home Assistant mobile app).
    * **Update Interval (Minutes):** How often to run the update.

---

### 2. Home Location Update - Distance

* **File:** `home_loc_update_distance.yaml`
* **Description:** Dynamically updates the core Home Assistant location when a geocoded sensor moves a specified distance from the *current* HA location. This is useful for filtering out GPS jitter while allowing the location to follow a device.
* **Inputs:**
    * **Geocoded Location Sensor:** The sensor providing location data.
    * **Update Threshold (Meters):** The distance the sensor must move before the location is updated.

---

## Installation

To use these blueprints in your Home Assistant instance:

1.  Go to **Settings > Automations & Scenes > Blueprints**.
2.  Click the **Import Blueprint** button.
3.  Paste the "Raw" URL of the blueprint you wish to import.

**Blueprint URLs:**

* **Timer:** `https://raw.githubusercontent.com/sambarlick/ha-blueprints/main/home_loc_update_timer.yaml`
* **Distance:** `https://raw.githubusercontent.com/sambarlick/ha-blueprints/main/home_loc_update_distance.yaml`

## License

This project is licensed under 
the MIT License.
