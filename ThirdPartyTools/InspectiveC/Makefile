ADDITIONAL_LDFLAGS  = -Wl,-segalign,4000
# ADDITIONAL_OBJCFLAGS += -S

TWEAK_NAME = InspectiveC
InspectiveC_FILES = hashmap.mm logging.mm blocks.mm InspectiveC.mm
InspectiveC_LIBRARIES = substrate
InspectiveC_FRAMEWORKS = Foundation UIKit

include theos/makefiles/common.mk
include $(THEOS_MAKE_PATH)/tweak.mk
include $(THEOS_MAKE_PATH)/library.mk

after-install::
	install.exec "killall -9 SpringBoard"
