## How to access the project
- make sure to be in a new directory
- git clone "repo-url"
- cd "directory-name"
- git remote -v (to make sure you have the correct remote for the url)
- git pull (should give you everything up to date)

## TASK1.grc
- generic sample rate 1M
- signal source (sin) with 1k freq (messanger)
- signal source (sin) with 10k freq (carrier)
- multiply them
- add to pluto SDR sink (give the sample rate manually because it accepts only integers)

## TASK2.grc
- generic sample rate of 48K 
  - to match the file source sampling rate 
  - measured file sample rate by an online tool)
- signal source (cos) with 10k freq (carrier)
- file source
- multiply them
- rational resampler to resample the sample rate to 1M
  - pluto SDR just accept 65k <= pluto <= idk forgot
  - 48k is less than 65k
- pluto SDR sink

## untitled.py
- idk tbh it just got here (i didn't write it)