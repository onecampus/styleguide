# Rails style guide of oncampus

### Params in view, controller and model

* `nil?` params[:id].nil? => true or false 多用
* `blank?` params[:ids].blank? 就等于 params[:ids].nil? || params[:ids].empty? 多用
* `present?` obj.present? => true if obj not blank 多用
* `empty?` array of hash is blank, [].empty? {}.empty? rails的`blank?`既判断了nil,又判断了empty,so用blank?
