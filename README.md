# WHALEINSIDE
De novo genome analysis

made by Song Dae Kwon

Run genome processing scripts. usage: whaleinside [-h] [-d /path/to/base] [-i /path/to/raw_1.fq.gz /path/to/raw_2.fq.gz] [-c /path/config_file]



'-d', '--directory', type=str, required=True, help='Base directory for input and output files.'

'-i', '--input', nargs=2, required=True, help='Paths to the raw input files.'

'-c', '--config', type=str, required=True, help='Path to the program configuration file.'

'-s', '--start-step', type=int, default=1, choices=[1, 2, 3, 4, 5, 6, 7],
                        help='Step to start the process from (default: 1; Trim: 1, ReadCheck: 2, Assembly: 3, Scaffold: 4, Prediction: 5, Estimation: 6, RepeatMasker: 7)'
