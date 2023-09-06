
root_path := ./../
own_path := ./

output_path := $(own_path)output/
src_path := $(root_path)src/

output_file_name := output.out

g++ := g++
flags := 

all:

	# Creates output directory if it does not exists
	mkdir output

	# Copies the main file into output path
	cp $(src_path)*.h $(src_path)*.cpp $(output_path) 

	# Copies example file into output path
	cp $(own_path)*.cpp $(output_path) 

	# Compile
	$(g++) $(flags) $(disable_warning_about_void_operations) $(output_path)*.cpp -o $(output_file_name)

	#Remove .h file
	rm $(output_path)*

	# Move output file into output directory
	mv $(output_file_name) $(output_path)
