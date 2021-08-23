










objects = hello 

all: $(objects)
$(objects): %: %.c
#模式规则使您可以使用make来编译需要相同编译命令的多个c文件
#%: %.c  目标 : 目标.c  目标 : 依赖  $@ $<    
	@echo debug1 = $@    
	@echo debug2 = $<    
	$(CC) $(CFLAGS) -o $@ $<    
	@echo debug3 = $<


.PHONY:clean


clean:    
	rm -rf $(objects)






