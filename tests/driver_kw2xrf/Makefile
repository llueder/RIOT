include ../Makefile.tests_common

BOARD_INSUFFICIENT_MEMORY := arduino-duemilanove arduino-leonardo \
                             arduino-mega2560 arduino-nano arduino-uno \
                             i-nucleo-lrwan1 nucleo-f031k6 nucleo-f042k6 \
                             nucleo-l031k6 nucleo-f334r8 nucleo-l053r8 \
                             stm32f0discovery stm32l0538-disco waspmote-pro

USEMODULE += auto_init_gnrc_netif
USEMODULE += gnrc_netdev_default
USEMODULE += shell
USEMODULE += shell_commands
USEMODULE += ps

DRIVER ?= kw2xrf

# finally include the actual chosen driver
USEMODULE += $(DRIVER)

include $(RIOTBASE)/Makefile.include
