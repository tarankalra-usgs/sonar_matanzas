1. ripple_wavelength-> The legacy code from Jordan that Dr. John Warner sent converted
to python by Gordon Leavitt 
Input -> rectangular image in rectangular coordinates
Output-> Wavelength and orientation of ripples

2. matlab_extraction_timestack-> Extracting teh smaller chunks of time stacked images in matlab. 
Input-> Data in form of rectangular images in netcdf file in rectangular coordinates
Ouput-> Time stacked .mat files with time on x axis and cross-shore movement of ripples on 

3. ripple_migration -> Division of the image in smaller chunks of time from Matanzas dataset
and then use of Canny edge algorithm in scikit package and use of OpenCV package to get the
migration of ripples. 
Input-> Time stacked .mat files with time on x axis and cross-shore movement of ripples on 
y axis
Ouput-> coordinates of time and cross-shore movement 

4. matlab_bedload_calc -> bedload calculation for each smaller chunk of time based on 
ripple wavelength and ripple migration rate 
Input -> Ripple characteristics, Ripple migration rates 
Output-> Bedload from Sonar 