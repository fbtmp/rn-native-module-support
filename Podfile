platform :ios, '12.4'
require_relative '../node_modules/react-native/scripts/react_native_pods'
require_relative '../node_modules/@react-native-community/cli-platform-ios/native_modules'

target 'RNLinearGradient' do
  config = use_native_modules!

  use_react_native!(:path => config[:reactNativePath])

  post_install do |installer|
    react_native_post_install(installer)
    __apply_Xcode_12_5_M1_post_install_workaround(installer)
  end
end
