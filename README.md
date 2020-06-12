#What's the Weather Like?
## Background

Whether financial, political, or social -- data's true power lies in its ability to answer questions definitively. So let's take what you've learned about Python requests, APIs, and JSON traversals to answer a fundamental question: "What's the weather like as we approach the equator?"

Now, we know what you may be thinking: _"Duh. It gets hotter..."/

# Part 1 

# Dependencies and Setup
import matplotlib.pyplot as plt
import pandas as pd
import numpy as np
import requests
import time
from scipy.stats import linregress
import json
import random
import scipy.stats as st
from citipy import citipy

# Import API key
from api_keys import weather_api_key

# Observations
1. Highest temperature is found at 0 latitude and as you move away from the equator, temperature decreases.
2. Southern Hemisphern climates tend to be slightly milder than in the Northen Hemisphere. 
3. Latitude does not have a strong correlation on wind speed. 
4. No relationship between Cloudiness and Latitude.
