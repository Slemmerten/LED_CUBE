################################################################################
# Automatically-generated file. Do not edit!
################################################################################

SHELL := cmd.exe
RM := rm -rf

USER_OBJS :=

LIBS := 
PROJ := 

O_SRCS := 
C_SRCS := 
S_SRCS := 
S_UPPER_SRCS := 
OBJ_SRCS := 
ASM_SRCS := 
PREPROCESSING_SRCS := 
OBJS := 
OBJS_AS_ARGS := 
C_DEPS := 
C_DEPS_AS_ARGS := 
EXECUTABLES := 
OUTPUT_FILE_PATH :=
OUTPUT_FILE_PATH_AS_ARGS :=
AVR_APP_PATH :=$$$AVR_APP_PATH$$$
QUOTE := "
ADDITIONAL_DEPENDENCIES:=
OUTPUT_FILE_DEP:=
LIB_DEP:=
LINKER_SCRIPT_DEP:=

# Every subdirectory with source files must be described here
SUBDIRS := 


# Add inputs and outputs from these tool invocations to the build variables 
C_SRCS +=  \
../Animations.c \
../Draw.c \
../main.c \
../Timers.c


PREPROCESSING_SRCS += 


ASM_SRCS += 


OBJS +=  \
Animations.o \
Draw.o \
main.o \
Timers.o

OBJS_AS_ARGS +=  \
Animations.o \
Draw.o \
main.o \
Timers.o

C_DEPS +=  \
Animations.d \
Draw.d \
main.d \
Timers.d

C_DEPS_AS_ARGS +=  \
Animations.d \
Draw.d \
main.d \
Timers.d

OUTPUT_FILE_PATH +=4x4x4_LED_Cube_Test_Circuit.elf

OUTPUT_FILE_PATH_AS_ARGS +=4x4x4_LED_Cube_Test_Circuit.elf

ADDITIONAL_DEPENDENCIES:=

OUTPUT_FILE_DEP:= ./makedep.mk

LIB_DEP+= 

LINKER_SCRIPT_DEP+= 


# AVR32/GNU C Compiler









./%.o: .././%.c
	@echo Building file: $<
	@echo Invoking: AVR/GNU C Compiler : 5.4.0
	$(QUOTE)F:\Marcus\software\Atmel Studio 7.0\7.0\toolchain\avr8\avr8-gnu-toolchain\bin\avr-gcc.exe$(QUOTE)  -x c -funsigned-char -funsigned-bitfields -DDEBUG  -I"F:\Marcus\software\Atmel Studio 7.0\7.0\Packs\atmel\ATmega_DFP\1.2.209\include"  -O1 -ffunction-sections -fdata-sections -fpack-struct -fshort-enums -mrelax -g2 -Wall -mmcu=atmega2560 -B "F:\Marcus\software\Atmel Studio 7.0\7.0\Packs\atmel\ATmega_DFP\1.2.209\gcc\dev\atmega2560" -c -std=gnu99 -MD -MP -MF "$(@:%.o=%.d)" -MT"$(@:%.o=%.d)" -MT"$(@:%.o=%.o)"   -o "$@" "$<" 
	@echo Finished building: $<
	



# AVR32/GNU Preprocessing Assembler



# AVR32/GNU Assembler




ifneq ($(MAKECMDGOALS),clean)
ifneq ($(strip $(C_DEPS)),)
-include $(C_DEPS)
endif
endif

# Add inputs and outputs from these tool invocations to the build variables 

# All Target
all: $(OUTPUT_FILE_PATH) $(ADDITIONAL_DEPENDENCIES)

$(OUTPUT_FILE_PATH): $(OBJS) $(USER_OBJS) $(OUTPUT_FILE_DEP) $(LIB_DEP) $(LINKER_SCRIPT_DEP)
	@echo Building target: $@
	@echo Invoking: AVR/GNU Linker : 5.4.0
	$(QUOTE)F:\Marcus\software\Atmel Studio 7.0\7.0\toolchain\avr8\avr8-gnu-toolchain\bin\avr-gcc.exe$(QUOTE) -o$(OUTPUT_FILE_PATH_AS_ARGS) $(OBJS_AS_ARGS) $(USER_OBJS) $(LIBS) -Wl,-Map="4x4x4_LED_Cube_Test_Circuit.map" -Wl,--start-group -Wl,-lm  -Wl,--end-group -Wl,--gc-sections -mrelax -mmcu=atmega2560 -B "F:\Marcus\software\Atmel Studio 7.0\7.0\Packs\atmel\ATmega_DFP\1.2.209\gcc\dev\atmega2560"  
	@echo Finished building target: $@
	"F:\Marcus\software\Atmel Studio 7.0\7.0\toolchain\avr8\avr8-gnu-toolchain\bin\avr-objcopy.exe" -O ihex -R .eeprom -R .fuse -R .lock -R .signature -R .user_signatures  "4x4x4_LED_Cube_Test_Circuit.elf" "4x4x4_LED_Cube_Test_Circuit.hex"
	"F:\Marcus\software\Atmel Studio 7.0\7.0\toolchain\avr8\avr8-gnu-toolchain\bin\avr-objcopy.exe" -j .eeprom  --set-section-flags=.eeprom=alloc,load --change-section-lma .eeprom=0  --no-change-warnings -O ihex "4x4x4_LED_Cube_Test_Circuit.elf" "4x4x4_LED_Cube_Test_Circuit.eep" || exit 0
	"F:\Marcus\software\Atmel Studio 7.0\7.0\toolchain\avr8\avr8-gnu-toolchain\bin\avr-objdump.exe" -h -S "4x4x4_LED_Cube_Test_Circuit.elf" > "4x4x4_LED_Cube_Test_Circuit.lss"
	"F:\Marcus\software\Atmel Studio 7.0\7.0\toolchain\avr8\avr8-gnu-toolchain\bin\avr-objcopy.exe" -O srec -R .eeprom -R .fuse -R .lock -R .signature -R .user_signatures "4x4x4_LED_Cube_Test_Circuit.elf" "4x4x4_LED_Cube_Test_Circuit.srec"
	"F:\Marcus\software\Atmel Studio 7.0\7.0\toolchain\avr8\avr8-gnu-toolchain\bin\avr-size.exe" "4x4x4_LED_Cube_Test_Circuit.elf"
	
	





# Other Targets
clean:
	-$(RM) $(OBJS_AS_ARGS) $(EXECUTABLES)  
	-$(RM) $(C_DEPS_AS_ARGS)   
	rm -rf "4x4x4_LED_Cube_Test_Circuit.elf" "4x4x4_LED_Cube_Test_Circuit.a" "4x4x4_LED_Cube_Test_Circuit.hex" "4x4x4_LED_Cube_Test_Circuit.lss" "4x4x4_LED_Cube_Test_Circuit.eep" "4x4x4_LED_Cube_Test_Circuit.map" "4x4x4_LED_Cube_Test_Circuit.srec" "4x4x4_LED_Cube_Test_Circuit.usersignatures"
	