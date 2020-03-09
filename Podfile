
platform :ios, '9.0'

inhibit_all_warnings!

source 'https://github.com/CocoaPods/Specs.git'

post_install do |installer|
    installer.pods_project.build_configurations.each do |config|
        if config.name.include?("Debug")
            config.build_settings['GCC_OPTIMIZATION_LEVEL'] = '0'
            if !config.build_settings['GCC_PREPROCESSOR_DEFINITIONS'].include?("DEBUG=1")
                config.build_settings['GCC_PREPROCESSOR_DEFINITIONS']<<'DEBUG=1'
            end
        end
    end
end

target 'NativeFlutterProject' do
    pod 'JLRoutes'


end

