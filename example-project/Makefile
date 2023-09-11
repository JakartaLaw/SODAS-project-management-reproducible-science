all: run-code compile-latex
	@echo "All tasks completed"

check-python:
	@python -c "import sys; print(sys.executable)"

clean-data:
	@jupyter nbconvert --to notebook --execute src/clean_data.ipynb

run-analysis:
	@jupyter nbconvert --to notebook --execute src/analysis.ipynb

remove-converted-notebooks:
	@rm src/*.nbconvert.ipynb

run-code: check-python clean-data run-analysis
	@echo "Generates all outputs"

compile-latex:
	@cd manuscript && pdflatex main.tex