# fsi-flexible-acc
This code simulates the fluid-structure interaction of a fully flexible filament immeresd in uniform flow. Plunge and pitch actuation can be provided at the leading edge of the filament.

# To run on a cluster (e.g. in the synchrony cluster available in the Biomemetics and Dynamic Lab IIT Madras, India):

// First load the GPU module using following command in terminal//

module load nvhpc/20.7

// Compile the souce_code //

pgc++ -o make.out -acc -Minfo=accel -ta=tesla:cc80 source_code.cpp


// Submit the code for simulation using run_IBMFSI.cmd //

qsub run_IBMFSI.cmd

