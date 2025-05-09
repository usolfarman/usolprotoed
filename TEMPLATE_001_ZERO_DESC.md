from python.render import render_template

def test_render_success():
    out = render_template('templates/TEMPLATE_001_ZERO_DESC.md', product_name='Test', features='fast CPU')
    assert 'Test' in out and 'fast CPU' in out