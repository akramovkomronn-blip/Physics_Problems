import math

# Given values
T_earth = 4  # seconds
g_earth = 9.8  # m/s^2
g_moon = g_earth / 6

# 1. Period on the Moon
T_moon = T_earth * math.sqrt(g_earth / g_moon)

# 2. Length for 1-second period on Earth
T_target = 1  # second
L = g_earth * (T_target / (2 * math.pi))**2

# Print results
print("Period on Moon:", round(T_moon, 2), "seconds")
print("Required length:", round(L, 3), "meters")
