# SCons hack to ignore unknown targets
import SCons.Script
SCons.Script.BUILD_TARGETS = ['.']

# SCons hack to ignore unknown options
import SCons.Script.Main
parser = SCons.Script.Main.OptionsParser
parser.largs = []
parser.rargs = []

# Nothing to do here
