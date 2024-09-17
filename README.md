# atmosphereclass Atmosphere:
    def __init__(self, temperature, pressure, oxygen_level):
        self.temperature = temperature      # Temperature in degrees Celsius
        self.pressure = pressure            # Pressure in Pascals (Pa)
        self.oxygen_level = oxygen_level    # Oxygen level as a percentage

    def set_temperature(self, new_temperature):
        self.temperature = new_temperature
        print(f"Temperature has been set to {self.temperature}°C.")

    def set_pressure(self, new_pressure):
        self.pressure = new_pressure
        print(f"Pressure has been set to {self.pressure} Pa.")

    def set_oxygen_level(self, new_oxygen_level):
        self.oxygen_level = new_oxygen_level
        print(f"Oxygen level has been set to {self.oxygen_level}%.")

    def describe(self):
        print(f"Current atmosphere: {self.temperature}°C, {self.pressure} Pa, Oxygen Level: {self.oxygen_level}%.")

# Example usage:
earth_atmosphere = Atmosphere(temperature=15, pressure=101325, oxygen_level=21)  # A typical Earth-like atmosphere
earth_atmosphere.describe()

earth_atmosphere.set_temperature(20)       # Set new temperature to 20°C
earth_atmosphere.set_pressure(100000)      # Adjust pressure to 100,000 Pa
earth_atmosphere.set_oxygen_level(19)      # Decrease oxygen level to 19%
earth_atmosphere.describe()                # Describe the updated atmosphere
