# 该 Makefile 用于编译一个 Beamer 制作的幻灯片
# 运行环境：Macunix, MacTex

Compiler = pdflatex
Reader = open

Target = beamer.pdf
Source = beamer.tex

TmpFile = *.out *.log *.aux *.nav *.snm *.toc *.gz

$(Target): $(Source)
	$(Compiler) $(Source)
	$(Compiler) $(Source)

all: $(Target) clean read 

read:
	$(Reader) $(Target)

clean:
	-rm $(TmpFile)

cleanall:
	-rm $(TmpFile) $(Target)

.PHONY: all read clean cleanall
